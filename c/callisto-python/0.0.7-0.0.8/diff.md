# Comparing `tmp/callisto-python-0.0.7.tar.gz` & `tmp/callisto-python-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/callisto-python-0.0.7.tar", last modified: Thu Apr  6 11:06:37 2023, max compression
+gzip compressed data, was "dist/callisto-python-0.0.8.tar", last modified: Fri Apr 21 02:01:22 2023, max compression
```

## Comparing `callisto-python-0.0.7.tar` & `callisto-python-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 teamcity  (1001) teamcity  (1001)        0 2023-04-06 11:06:37.000000 callisto-python-0.0.7/
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)       43 2023-02-16 17:57:49.000000 callisto-python-0.0.7/README.md
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)      811 2023-02-16 17:57:49.000000 callisto-python-0.0.7/setup.py
-drwxr-xr-x   0 teamcity  (1001) teamcity  (1001)        0 2023-04-06 11:06:37.000000 callisto-python-0.0.7/callisto_python.egg-info/
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)       36 2023-04-06 11:06:37.000000 callisto-python-0.0.7/callisto_python.egg-info/requires.txt
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)      395 2023-04-06 11:06:37.000000 callisto-python-0.0.7/callisto_python.egg-info/SOURCES.txt
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)        1 2023-04-06 11:06:37.000000 callisto-python-0.0.7/callisto_python.egg-info/dependency_links.txt
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)        9 2023-04-06 11:06:37.000000 callisto-python-0.0.7/callisto_python.egg-info/top_level.txt
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)      506 2023-04-06 11:06:37.000000 callisto-python-0.0.7/callisto_python.egg-info/PKG-INFO
-drwxr-xr-x   0 teamcity  (1001) teamcity  (1001)        0 2023-04-06 11:06:37.000000 callisto-python-0.0.7/callisto/
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)       88 2023-04-06 11:05:41.000000 callisto-python-0.0.7/callisto/version.py
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)      130 2023-02-16 17:57:49.000000 callisto-python-0.0.7/callisto/command.py
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)     1976 2023-03-23 12:33:49.000000 callisto-python-0.0.7/callisto/pandas_statistics.py
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)     1770 2023-02-16 17:57:49.000000 callisto-python-0.0.7/callisto/download.py
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)    27644 2023-02-27 13:17:00.000000 callisto-python-0.0.7/callisto/var_utils.py
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)      518 2023-02-16 17:57:49.000000 callisto-python-0.0.7/callisto/notification.py
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)     2676 2023-04-06 10:21:46.000000 callisto-python-0.0.7/callisto/stats_utils.py
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)      423 2023-03-07 15:42:30.000000 callisto-python-0.0.7/callisto/__init__.py
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)       38 2023-04-06 11:06:37.000000 callisto-python-0.0.7/setup.cfg
--rw-r--r--   0 teamcity  (1001) teamcity  (1001)      506 2023-04-06 11:06:37.000000 callisto-python-0.0.7/PKG-INFO
+drwxr-xr-x   0 teamcity  (1001) teamcity  (1001)        0 2023-04-21 02:01:22.000000 callisto-python-0.0.8/
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)       43 2023-02-16 17:57:49.000000 callisto-python-0.0.8/README.md
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)      877 2023-04-11 21:31:58.000000 callisto-python-0.0.8/setup.py
+drwxr-xr-x   0 teamcity  (1001) teamcity  (1001)        0 2023-04-21 02:01:22.000000 callisto-python-0.0.8/callisto_python.egg-info/
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)       63 2023-04-21 02:01:22.000000 callisto-python-0.0.8/callisto_python.egg-info/requires.txt
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)      395 2023-04-21 02:01:22.000000 callisto-python-0.0.8/callisto_python.egg-info/SOURCES.txt
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)        1 2023-04-21 02:01:22.000000 callisto-python-0.0.8/callisto_python.egg-info/dependency_links.txt
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)        9 2023-04-21 02:01:22.000000 callisto-python-0.0.8/callisto_python.egg-info/top_level.txt
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)      529 2023-04-21 02:01:22.000000 callisto-python-0.0.8/callisto_python.egg-info/PKG-INFO
+drwxr-xr-x   0 teamcity  (1001) teamcity  (1001)        0 2023-04-21 02:01:22.000000 callisto-python-0.0.8/callisto/
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)       88 2023-04-11 21:34:34.000000 callisto-python-0.0.8/callisto/version.py
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)      130 2023-02-16 17:57:49.000000 callisto-python-0.0.8/callisto/command.py
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)     2135 2023-04-21 01:26:03.000000 callisto-python-0.0.8/callisto/pandas_statistics.py
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)     1770 2023-02-16 17:57:49.000000 callisto-python-0.0.8/callisto/download.py
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)    29402 2023-04-21 01:26:03.000000 callisto-python-0.0.8/callisto/var_utils.py
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)      518 2023-02-16 17:57:49.000000 callisto-python-0.0.8/callisto/notification.py
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)     2541 2023-04-11 20:42:55.000000 callisto-python-0.0.8/callisto/stats_utils.py
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)      423 2023-03-07 15:42:30.000000 callisto-python-0.0.8/callisto/__init__.py
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)       38 2023-04-21 02:01:22.000000 callisto-python-0.0.8/setup.cfg
+-rw-r--r--   0 teamcity  (1001) teamcity  (1001)      529 2023-04-21 02:01:22.000000 callisto-python-0.0.8/PKG-INFO
```

### Comparing `callisto-python-0.0.7/setup.py` & `callisto-python-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,8 +23,11 @@
         "Operating System :: OS Independent",
     ],
     python_requires='>=3',
     install_requires=[
         "requests>=2.28.1,<3",
         "tqdm>=4.64.0,<5",
     ],
+    extras_require={
+        "pandas": ["pandas>=1.0.0,<3"]
+    }
 )
```

### Comparing `callisto-python-0.0.7/callisto/pandas_statistics.py` & `callisto-python-0.0.8/callisto/pandas_statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import pandas as pd  # type: ignore
 from pandas.api.types import is_categorical_dtype  # type: ignore
 from pandas.api.types import is_datetime64_any_dtype, is_numeric_dtype
 
 
 def get_single_column_stats(col, n_top_values):
+    if type(col).__name__ != "Series":
+        col = pd.Series(col)
+
     series_stats = {}
     series_stats["na_count"] = int(col.isna().sum())
 
     if is_numeric_dtype(col):
         series_stats["type"] = "numeric"
         series_stats["min"] = col.min()
         series_stats["max"] = col.max()
@@ -57,7 +60,11 @@
     if isinstance(col.dtype, pd.StringDtype):
         return True
     elif col.dtype == "object":
         # Object series, check each value
         return all((v is None) or isinstance(v, str) for v in col)
     else:
         return False
+
+
+def get_schema_type(s):
+    return pd.io.json._table_schema.as_json_table_type(s.dtype)
```

### Comparing `callisto-python-0.0.7/callisto/download.py` & `callisto-python-0.0.8/callisto/download.py`

 * *Files identical despite different names*

### Comparing `callisto-python-0.0.7/callisto/var_utils.py` & `callisto-python-0.0.8/callisto/var_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import json
 import sys
 import traceback
 
-import numpy as np  # type: ignore
+try:
+    import numpy as np  # type: ignore
+except Exception:
+    np = None
 
 KB = float(1024)
 MB = float(KB ** 2)  # 1,048,576
 GB = float(KB ** 3)  # 1,073,741,824
 TB = float(KB ** 4)  # 1,099,511,627,776
 
 DEFAULT_PAGE_SIZE = 50
+MAX_SINGLE_VALUE_LENGTH = 500
+MAX_SUMMARY_LENGTH = 140
 
 
 def human_bytes(B):
     """Return the given bytes as a human friendly KB, MB, GB, or TB string"""
     B = float(B)
 
     if B < KB:
@@ -24,29 +29,32 @@
         return "{0:.2f} MB".format(B / MB)
     elif GB <= B < TB:
         return "{0:.2f} GB".format(B / GB)
     elif TB <= B:
         return "{0:.2f} TB".format(B / TB)
 
 
-def make_multi_dict(row_names, column_names, data, total_row_count, total_column_count):
+def make_multi_dict(
+    row_names, column_names, data, total_row_count, total_column_count, column_types
+):
     """
     column_count and row_count should be values for the whole data structure
     column_names and row_names are values for the possibly abbreviated structure
     """
     if type(column_names) == str:
         column_names = [column_names]
     if type(row_names) == str:
         row_names == [row_names]
     value = {
         "column_count": total_column_count,
         "row_count": total_row_count,
         "column_names": column_names,
         "row_names": row_names,
         "data": data,
+        "column_types": column_types,
     }
     return {"multi_value": value}
 
 
 def validate_value(value, no_preview=False):
     if value is None and no_preview:
         return None
@@ -54,14 +62,16 @@
         return {"single_value": str(value["single_value"])}
     elif list(value.keys()) == ["multi_value"]:
         val = value["multi_value"]
         if val["column_names"] is not None:
             val["column_names"] = list(map(str, val["column_names"]))
         if val["row_names"] is not None:
             val["row_names"] = list(map(str, val["row_names"]))
+        if val["column_types"] is not None:
+            val["column_types"] = list(map(str, val["column_types"]))
         if val["data"] is not None:
             # double map through the nested arrays in 'data'
             val["data"] = list(map(lambda x: list(map(str, x)), val["data"]))
         return {"multi_value": val}
     else:
         msg = (
             "Value should be single entry dict with a key of "
@@ -139,18 +149,24 @@
         row_names = list(range(start, end))
         preview = make_multi_dict(
             row_names,
             name,
             data,
             total_row_count=len(obj_filtered),
             total_column_count=1,
+            column_types=None,
         )
     else:
         preview = make_multi_dict(
-            None, None, None, total_row_count=len(obj), total_column_count=1
+            None,
+            None,
+            None,
+            total_row_count=len(obj),
+            total_column_count=1,
+            column_types=None,
         )
     return (
         summary,
         has_next_page,
         preview,
     )
 
@@ -242,18 +258,24 @@
         row_names = list(range(start, end))
         preview = make_multi_dict(
             row_names,
             ["Key", "Value"],
             data,
             total_row_count=len(obj_filtered),
             total_column_count=2,
+            column_types=None,
         )
     else:
         preview = make_multi_dict(
-            None, None, None, total_row_count=len(obj), total_column_count=2
+            None,
+            None,
+            None,
+            total_row_count=len(obj),
+            total_column_count=2,
+            column_types=None,
         )
     return (
         summary,
         has_next_page,
         preview,
     )
 
@@ -267,14 +289,16 @@
     ascending=None,
     filters=None,
 ):
     """
     sort_by: list of indexes (integers) to sort
     ascending: expects a list with single boolean
     """
+    from .pandas_statistics import get_schema_type
+
     summary = f"Size: {obj.shape[0]}x{obj.shape[1]} Memory: {human_bytes(obj.nbytes)}"
     has_next_page = False
     preview = None
     if not no_preview:
 
         if filters and isinstance(filters, list):
             obj_filtered = obj.copy()
@@ -347,24 +371,35 @@
         else:
             obj_sorted = obj_filtered
 
         obj_pre = obj_sorted[start:end]
         data = obj_pre.tolist()
         row_names = list(range(start, end))
         column_names = list(range(obj_pre.shape[1]))
+
+        column_types = []
+        for col in range(obj.shape[1]):
+            column_types.append(get_schema_type(obj[:, col]))
+
         preview = make_multi_dict(
-            row_names, column_names, data, obj_filtered.shape[0], obj_filtered.shape[1]
+            row_names,
+            column_names,
+            data,
+            obj_filtered.shape[0],
+            obj_filtered.shape[1],
+            column_types=column_types,
         )
     else:
         preview = make_multi_dict(
             None,
             None,
             None,
             total_row_count=obj.shape[0],
             total_column_count=obj.shape[1],
+            column_types=None,
         )
     return (
         summary,
         has_next_page,
         preview,
     )
 
@@ -375,14 +410,16 @@
     no_preview=False,
     page_size=DEFAULT_PAGE_SIZE,
     page=0,
     sort_by=None,
     ascending=None,
     filters=None,
 ):
+    from .pandas_statistics import get_schema_type
+
     summary = f"Length: {obj.shape[0]} Memory: {human_bytes(obj.nbytes)}"
     has_next_page = False
     preview = None
     if not no_preview:
 
         if filters and isinstance(filters, list):
             obj_filtered = obj.copy()
@@ -459,24 +496,33 @@
         else:
             obj_sorted = obj_filtered
 
         obj_pre = obj_sorted[start:end]
         data = tuple(map(lambda x: [str(x)], obj_pre.tolist()))
         row_names = list(range(start, end))
         column_names = name
+
+        column_types = [get_schema_type(obj)]
+
         preview = make_multi_dict(
             row_names,
             column_names,
             data,
             total_row_count=obj_filtered.shape[0],
             total_column_count=1,
+            column_types=column_types,
         )
     else:
         preview = make_multi_dict(
-            None, None, None, total_row_count=obj.shape[0], total_column_count=1
+            None,
+            None,
+            None,
+            total_row_count=obj.shape[0],
+            total_column_count=1,
+            column_types=None,
         )
     return (
         summary,
         has_next_page,
         preview,
     )
 
@@ -490,18 +536,17 @@
     ascending=None,
     filters=None,
 ):
     """
     sort_by: list of strings (names of columns to sort), or ["index"] to sort by index
     ascending: list of booleans (must match length of sort_by), or single boolean
     """
-    summary = (
-        f"Size: {obj.shape[0]}x{obj.shape[1]}"
-        + f" Memory: {human_bytes(obj.memory_usage(deep=True).sum())}"
-    )
+    from .pandas_statistics import get_schema_type
+
+    summary = f"Size: {obj.shape[0]}x{obj.shape[1]}"
     has_next_page = False
     preview = None
     if not no_preview:
 
         if filters and isinstance(filters, list):
             obj_filtered = obj.copy()
             for filter in filters:
@@ -559,24 +604,36 @@
             obj_sorted = obj_filtered
 
         obj_pre = obj_sorted.iloc[start:end]
 
         data = obj_pre.to_numpy().tolist()
         row_names = tuple(map(lambda x: str(x), obj_pre.index.to_list()))
         column_names = obj_pre.columns.to_list()
+
+        column_types = []
+        for col_name, col in obj.items():
+            column_types.append(get_schema_type(col))
+
         preview = make_multi_dict(
-            row_names, column_names, data, obj_filtered.shape[0], obj_filtered.shape[1]
+            row_names,
+            column_names,
+            data,
+            obj_filtered.shape[0],
+            obj_filtered.shape[1],
+            column_types,
         )
+
     else:
         preview = make_multi_dict(
             None,
             None,
             None,
             total_row_count=obj.shape[0],
             total_column_count=obj.shape[1],
+            column_types=None,
         )
     return (
         summary,
         has_next_page,
         preview,
     )
 
@@ -591,15 +648,17 @@
     ascending=None,
     filters=None,
 ):
     """
     sort_by: list of strings (either "index" or "value")
     ascending: expects a list with a single boolean
     """
-    summary = f"Length: {len(obj)} Memory: {human_bytes(obj.memory_usage(deep=True))}"
+    from .pandas_statistics import get_schema_type
+
+    summary = f"Length: {len(obj)}"
     has_next_page = False
     preview = None
     if not no_preview:
 
         if filters and isinstance(filters, list):
             obj_filtered = obj.copy()
             filter = filters[0]
@@ -669,24 +728,34 @@
                 obj_sorted = obj_filtered
         else:
             obj_sorted = obj_filtered
 
         obj_pre = obj_sorted.iloc[start:end]
         data = tuple(map(lambda x: [str(x)], obj_pre.to_list()))
         row_names = tuple(map(lambda x: str(x), obj_pre.index.to_list()))
+
+        column_types = [get_schema_type(obj)]
+
         preview = make_multi_dict(
             row_names,
             name,
             data,
             total_row_count=obj_filtered.size,
             total_column_count=1,
+            column_types=column_types,
         )
+
     else:
         preview = make_multi_dict(
-            None, None, None, total_row_count=obj.size, total_column_count=1
+            None,
+            None,
+            None,
+            total_row_count=obj.size,
+            total_column_count=1,
+            column_types=None,
         )
     return (
         summary,
         has_next_page,
         preview,
     )
 
@@ -724,18 +793,24 @@
             getattr(obj, "jupyter_d1_value")
         ):
             value = obj.jupyter_d1_value()
         else:
             value = None
 
     # single valued intrinsics
-    elif obj_type.__name__ in ["int", "str", "float", "bool", "complex"]:
+    elif obj_type.__name__ in ["int", "float", "bool", "complex"]:
         summary = obj
         value = {"single_value": str(obj)}
+    elif obj_type.__name__ in ["str", "bytes"]:
+        if no_preview and len(obj) > MAX_SINGLE_VALUE_LENGTH:
+            summary = str(obj[:MAX_SINGLE_VALUE_LENGTH])
+        else:
+            summary = str(obj)
 
+        value = {"single_value": summary}
     # list
     elif obj_type.__name__ == "list" or obj_type.__name__ == "tuple":
         summary, has_next_page, value = get_list_var(
             obj,
             name,
             no_preview,
             page_size=page_size,
@@ -806,21 +881,23 @@
             ascending=ascending,
             filters=filters,
         )
 
     # if all else fails, fall back to single value string representation
     else:
         summary = str(obj)
-        value = {"single_value": str(obj)}
+        if no_preview and len(summary) > MAX_SINGLE_VALUE_LENGTH:
+            summary = summary[:MAX_SINGLE_VALUE_LENGTH]
+        value = {"single_value": summary}
 
     return {
         "name": name,
         "type": obj_type.__name__,
         "has_next_page": bool(has_next_page),
-        "summary": str(summary)[:140],  # limit summary length
+        "summary": str(summary)[:MAX_SUMMARY_LENGTH],  # limit summary length
         "value": validate_value(value, no_preview),
     }
 
 
 def create_exception_var(e):
     exc_type, exc_value, exc_tb = sys.exc_info()
     traceback_lines = traceback.format_exception(exc_type, exc_value, exc_tb)
```

### Comparing `callisto-python-0.0.7/callisto/notification.py` & `callisto-python-0.0.8/callisto/notification.py`

 * *Files identical despite different names*

### Comparing `callisto-python-0.0.7/callisto/stats_utils.py` & `callisto-python-0.0.8/callisto/stats_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import json
 import sys
 import traceback
 
-import pandas as pd  # type: ignore
-
-from .pandas_statistics import get_single_column_stats
-
 # Return this many of the most common values from a categorical column
 DEFAULT_TOP_VALUES = 3
 
 
 def create_exception_stats(e):
     exc_type, exc_value, exc_tb = sys.exc_info()
     traceback_lines = traceback.format_exception(exc_type, exc_value, exc_tb)
@@ -18,14 +14,16 @@
         "type": type(e).__name__,
         "summary": str(e),
         "error": tuple(map(lambda x: [x], traceback_lines)),
     }
 
 
 def get_stat_summary(obj, name, column):
+    from .pandas_statistics import get_single_column_stats
+
     obj_type = type(obj)
     stats = {}
 
     # pandas dataframe
     if obj_type.__name__ == "DataFrame":
         if column is None:
             for col_name in obj:
@@ -36,40 +34,38 @@
             stats[column] = get_single_column_stats(col, DEFAULT_TOP_VALUES)
     # pandas series
     elif obj_type.__name__ == "Series":
         stats[name] = get_single_column_stats(obj, DEFAULT_TOP_VALUES)
 
     # numpy 1d array
     elif obj_type.__name__ == "ndarray" and obj.ndim == 1:
-        col = pd.Series(obj)
-        stats["0"] = get_single_column_stats(col, DEFAULT_TOP_VALUES)
+        stats["0"] = get_single_column_stats(obj, DEFAULT_TOP_VALUES)
 
     # numpy 2d array
     elif obj_type.__name__ == "ndarray" and obj.ndim == 2:
         if column is None:
             for col_index in range(0, obj.shape[1]):
                 col_name = col_index
-                col = pd.Series(obj[:, col_index])
+                col = obj[:, col_index]
                 stats[col_name] = get_single_column_stats(col, DEFAULT_TOP_VALUES)
         else:
             column_int = int(column)
             if column_int >= 0 and column_int < obj.shape[1]:
-                col = pd.Series(obj[:, column_int])
+                col = obj[:, column_int]
                 stats[column] = get_single_column_stats(col, DEFAULT_TOP_VALUES)
     # list
     elif obj_type.__name__ == "list" or obj_type.__name__ == "tuple":
-        col = pd.Series(obj)
-        stats[name] = get_single_column_stats(col, DEFAULT_TOP_VALUES)
+        stats[name] = get_single_column_stats(obj, DEFAULT_TOP_VALUES)
 
     # dictionary
     elif obj_type.__name__ == "dict":
-        keys = pd.Series(list(obj.keys()))
+        keys = list(obj.keys())
         stats["Key"] = get_single_column_stats(keys, DEFAULT_TOP_VALUES)
 
-        values = pd.Series(list(obj.values()))
+        values = list(obj.values())
         stats["Value"] = get_single_column_stats(values, DEFAULT_TOP_VALUES)
 
     return stats
 
 
 def get_var_stats(
     obj,
```

