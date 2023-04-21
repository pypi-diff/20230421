# Comparing `tmp/iql-0.1.6-py3-none-any.whl.zip` & `tmp/iql-0.1.9b5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,55 +1,27 @@
-Zip file size: 75243 bytes, number of entries: 53
--rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-02 22:33 examples/__init__.py
--rw-rw-rw-  2.0 fat      265 b- defN 23-Mar-09 21:55 iql/__init__.py
--rw-rw-rw-  2.0 fat      431 b- defN 23-Mar-02 21:54 iql/config.ini
--rw-rw-rw-  2.0 fat     3301 b- defN 23-Mar-02 23:33 iql/initializer.py
--rw-rw-rw-  2.0 fat    26884 b- defN 23-Mar-09 21:24 iql/iqmoql.py
--rw-rw-rw-  2.0 fat     1226 b- defN 23-Mar-08 19:28 iql/options_parser.py
--rw-rw-rw-  2.0 fat     2951 b- defN 23-Mar-08 19:28 iql/q_cache.py
--rw-rw-rw-  2.0 fat       79 b- defN 23-Mar-08 19:28 iql/bbg_bql/__init__.py
--rw-rw-rw-  2.0 fat    10096 b- defN 23-Mar-09 21:09 iql/bbg_bql/bql_datamodel.py
--rw-rw-rw-  2.0 fat    14061 b- defN 23-Mar-09 02:35 iql/bbg_bql/bql_extension.py
--rw-rw-rw-  2.0 fat    13065 b- defN 23-Mar-09 21:22 iql/bbg_bql/bql_wrapper.py
--rw-rw-rw-  2.0 fat      692 b- defN 23-Mar-08 19:28 iql/bbg_bql/debug_tools.py
--rw-rw-rw-  2.0 fat       79 b- defN 23-Mar-08 19:28 iql/db_connectors/__init__.py
--rw-rw-rw-  2.0 fat     1651 b- defN 23-Mar-08 19:28 iql/db_connectors/duckdb_connector.py
--rw-rw-rw-  2.0 fat       79 b- defN 23-Mar-08 19:28 iql/extensions/__init__.py
--rw-rw-rw-  2.0 fat     3101 b- defN 23-Mar-09 21:42 iql/extensions/aws_s3_extension.py
--rw-rw-rw-  2.0 fat     7850 b- defN 23-Mar-09 02:17 iql/extensions/edgar_extension.py
--rw-rw-rw-  2.0 fat     4288 b- defN 23-Mar-08 19:28 iql/extensions/fred_extension.py
--rw-rw-rw-  2.0 fat     4087 b- defN 23-Mar-08 19:28 iql/extensions/kaggle_extension.py
--rw-rw-rw-  2.0 fat     1303 b- defN 23-Mar-08 19:28 iql/extensions/pandas_extension.py
--rw-rw-rw-  2.0 fat     1267 b- defN 23-Mar-08 19:28 iql/extensions/rest_api_extension.py
--rw-rw-rw-  2.0 fat     1297 b- defN 23-Mar-09 21:36 iql/extensions/sklearn_extension.py
--rw-rw-rw-  2.0 fat      773 b- defN 23-Mar-09 21:21 iql/extensions/template_extension.py
--rw-rw-rw-  2.0 fat       83 b- defN 23-Mar-02 22:37 src/__init__.py
--rw-rw-rw-  2.0 fat     2823 b- defN 23-Mar-02 21:55 src/initializer.py
--rw-rw-rw-  2.0 fat     7928 b- defN 23-Mar-02 22:16 src/iqmoql.py
--rw-rw-rw-  2.0 fat     2314 b- defN 23-Mar-01 14:38 src/q_cache.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-02 22:35 src/bbg_bql/__init__.py
--rw-rw-rw-  2.0 fat    10041 b- defN 23-Mar-02 01:20 src/bbg_bql/bql_datamodel.py
--rw-rw-rw-  2.0 fat    18689 b- defN 23-Mar-02 14:49 src/bbg_bql/bql_extension.py
--rw-rw-rw-  2.0 fat    11287 b- defN 23-Mar-02 16:23 src/bbg_bql/bql_wrapper.py
--rw-rw-rw-  2.0 fat      637 b- defN 23-Mar-01 23:10 src/bbg_bql/debug_tools.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-02 22:33 src/db_connectors/__init__.py
--rw-rw-rw-  2.0 fat     1062 b- defN 23-Mar-02 16:09 src/db_connectors/duckdb_connector.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-02 22:33 src/examples/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-02 22:33 src/extensions/__init__.py
--rw-rw-rw-  2.0 fat     1753 b- defN 23-Mar-02 21:51 src/extensions/aws_s3_extension.py
--rw-rw-rw-  2.0 fat     1887 b- defN 23-Mar-02 21:01 src/extensions/fred_extension.py
--rw-rw-rw-  2.0 fat     3085 b- defN 23-Mar-02 21:00 src/extensions/kaggle_extension.py
--rw-rw-rw-  2.0 fat     2713 b- defN 23-Mar-02 15:58 src/extensions/rest_api_extension.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-02 22:43 src/tests/__init__.py
--rw-rw-rw-  2.0 fat      212 b- defN 23-Mar-01 00:43 src/tests/conftest.py
--rw-rw-rw-  2.0 fat      496 b- defN 23-Mar-01 15:47 src/tests/test_bql_extension.py
--rw-rw-rw-  2.0 fat     7104 b- defN 23-Feb-28 16:35 src/tests/test_bql_wrapper.py
--rw-rw-rw-  2.0 fat     1693 b- defN 23-Mar-01 02:36 src/tests/test_iqmoql 2.py
--rw-rw-rw-  2.0 fat     5241 b- defN 23-Mar-01 02:22 src/tests/test_iqmoql_bql.py
--rw-rw-rw-  2.0 fat     1095 b- defN 23-Mar-01 02:38 src/tests/test_iqmoql_s3api.py
--rw-rw-rw-  2.0 fat     1679 b- defN 23-Mar-01 02:38 src/tests/test_iqmoql_sql.py
--rw-rw-rw-  2.0 fat      535 b- defN 23-Mar-09 21:56 iql-0.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    25571 b- defN 23-Mar-09 21:56 iql-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-09 21:56 iql-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Mar-09 21:56 iql-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     4344 b- defN 23-Mar-09 21:56 iql-0.1.6.dist-info/RECORD
-53 files, 211194 bytes uncompressed, 68377 bytes compressed:  67.6%
+Zip file size: 47431 bytes, number of entries: 25
+-rw-r--r--  2.0 unx      334 b- defN 23-Apr-21 12:33 iql/__init__.py
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-21 12:34 iql/_version.py
+-rw-r--r--  2.0 unx    34700 b- defN 23-Apr-21 12:33 iql/iqmoql.py
+-rw-r--r--  2.0 unx     1282 b- defN 23-Apr-21 12:33 iql/options_parser.py
+-rw-r--r--  2.0 unx     3233 b- defN 23-Apr-21 12:33 iql/q_cache.py
+-rw-r--r--  2.0 unx     2191 b- defN 23-Apr-21 12:33 iql/threading_experimental.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Apr-21 12:33 iql/bbg_bql/__init__.py
+-rw-r--r--  2.0 unx    10069 b- defN 23-Apr-21 12:33 iql/bbg_bql/bql_datamodel.py
+-rw-r--r--  2.0 unx     8975 b- defN 23-Apr-21 12:33 iql/bbg_bql/bql_extension.py
+-rw-r--r--  2.0 unx    13694 b- defN 23-Apr-21 12:33 iql/bbg_bql/bql_wrapper.py
+-rw-r--r--  2.0 unx      692 b- defN 23-Apr-21 12:33 iql/bbg_bql/debug_tools.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Apr-21 12:33 iql/db_connectors/__init__.py
+-rw-r--r--  2.0 unx     3253 b- defN 23-Apr-21 12:33 iql/db_connectors/duckdb_connector.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Apr-21 12:33 iql/extensions/__init__.py
+-rw-r--r--  2.0 unx     3470 b- defN 23-Apr-21 12:33 iql/extensions/aws_s3_extension.py
+-rw-r--r--  2.0 unx     7829 b- defN 23-Apr-21 12:33 iql/extensions/edgar_extension.py
+-rw-r--r--  2.0 unx     4279 b- defN 23-Apr-21 12:33 iql/extensions/fred_extension.py
+-rw-r--r--  2.0 unx     4106 b- defN 23-Apr-21 12:33 iql/extensions/kaggle_extension.py
+-rw-r--r--  2.0 unx     2315 b- defN 23-Apr-21 12:33 iql/extensions/pandas_extension.py
+-rw-r--r--  2.0 unx      666 b- defN 23-Apr-21 12:33 iql/extensions/template_extension.py
+-rw-r--r--  2.0 unx      535 b- defN 23-Apr-21 12:34 iql-0.1.9b5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    27298 b- defN 23-Apr-21 12:34 iql-0.1.9b5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 12:34 iql-0.1.9b5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-21 12:34 iql-0.1.9b5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2041 b- defN 23-Apr-21 12:34 iql-0.1.9b5.dist-info/RECORD
+25 files, 131392 bytes uncompressed, 44145 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -1,28 +1,25 @@
-Filename: examples/__init__.py
-Comment: 
-
 Filename: iql/__init__.py
 Comment: 
 
-Filename: iql/config.ini
-Comment: 
-
-Filename: iql/initializer.py
+Filename: iql/_version.py
 Comment: 
 
 Filename: iql/iqmoql.py
 Comment: 
 
 Filename: iql/options_parser.py
 Comment: 
 
 Filename: iql/q_cache.py
 Comment: 
 
+Filename: iql/threading_experimental.py
+Comment: 
+
 Filename: iql/bbg_bql/__init__.py
 Comment: 
 
 Filename: iql/bbg_bql/bql_datamodel.py
 Comment: 
 
 Filename: iql/bbg_bql/bql_extension.py
@@ -54,107 +51,26 @@
 
 Filename: iql/extensions/kaggle_extension.py
 Comment: 
 
 Filename: iql/extensions/pandas_extension.py
 Comment: 
 
-Filename: iql/extensions/rest_api_extension.py
-Comment: 
-
-Filename: iql/extensions/sklearn_extension.py
-Comment: 
-
 Filename: iql/extensions/template_extension.py
 Comment: 
 
-Filename: src/__init__.py
-Comment: 
-
-Filename: src/initializer.py
-Comment: 
-
-Filename: src/iqmoql.py
-Comment: 
-
-Filename: src/q_cache.py
-Comment: 
-
-Filename: src/bbg_bql/__init__.py
-Comment: 
-
-Filename: src/bbg_bql/bql_datamodel.py
-Comment: 
-
-Filename: src/bbg_bql/bql_extension.py
-Comment: 
-
-Filename: src/bbg_bql/bql_wrapper.py
-Comment: 
-
-Filename: src/bbg_bql/debug_tools.py
-Comment: 
-
-Filename: src/db_connectors/__init__.py
-Comment: 
-
-Filename: src/db_connectors/duckdb_connector.py
-Comment: 
-
-Filename: src/examples/__init__.py
-Comment: 
-
-Filename: src/extensions/__init__.py
-Comment: 
-
-Filename: src/extensions/aws_s3_extension.py
-Comment: 
-
-Filename: src/extensions/fred_extension.py
-Comment: 
-
-Filename: src/extensions/kaggle_extension.py
-Comment: 
-
-Filename: src/extensions/rest_api_extension.py
-Comment: 
-
-Filename: src/tests/__init__.py
-Comment: 
-
-Filename: src/tests/conftest.py
-Comment: 
-
-Filename: src/tests/test_bql_extension.py
-Comment: 
-
-Filename: src/tests/test_bql_wrapper.py
-Comment: 
-
-Filename: src/tests/test_iqmoql 2.py
-Comment: 
-
-Filename: src/tests/test_iqmoql_bql.py
-Comment: 
-
-Filename: src/tests/test_iqmoql_s3api.py
-Comment: 
-
-Filename: src/tests/test_iqmoql_sql.py
-Comment: 
-
-Filename: iql-0.1.6.dist-info/LICENSE
+Filename: iql-0.1.9b5.dist-info/LICENSE
 Comment: 
 
-Filename: iql-0.1.6.dist-info/METADATA
+Filename: iql-0.1.9b5.dist-info/METADATA
 Comment: 
 
-Filename: iql-0.1.6.dist-info/WHEEL
+Filename: iql-0.1.9b5.dist-info/WHEEL
 Comment: 
 
-Filename: iql-0.1.6.dist-info/top_level.txt
+Filename: iql-0.1.9b5.dist-info/top_level.txt
 Comment: 
 
-Filename: iql-0.1.6.dist-info/RECORD
+Filename: iql-0.1.9b5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iql/__init__.py

```diff
@@ -1,12 +1,16 @@
 # Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
 # All Rights Reserved
+from multiprocessing import Process, log_to_stderr
 
 from iql.iqmoql import (
     execute,
-    activate_cache,
+    configure,
     get_extension,
     list_extensions,
     register_extension,
-    DEFAULT_EXT_DIRECTORY
 )
 from iql.q_cache import clear_caches
+
+# import logging
+
+# log_to_stderr(logging.INFO)
```

## iql/iqmoql.py

```diff
@@ -3,96 +3,220 @@
 
 import logging
 import sqlparse
 import importlib
 import os
 import re
 from dataclasses import dataclass, field
-from typing import List, Dict, Optional, Union, Tuple
+from typing import List, Dict, Optional, Union, Tuple, Callable
 from pandas import DataFrame
+from pyarrow import Table
 import pandas as pd
 from abc import abstractmethod
 from iql import q_cache as qc
 from iql import options_parser
+from iql import threading_experimental as te
 
-last_real_name = False
-
-
-# DB_MODULE is loaded on first call to get_dbmodule()
-# Replace this string with another connector prior to first use,
-# or set _DBCONNECTOR to None after changing.
-DB_MODULE: str = "iql.db_connectors.duckdb_connector"
 
 # Cache Settings
 # Use iqmoql.activate_cache() before first execute() to
 # ensure settings propogate to individual extensions.
 # Infinite in memory cache by default
 _CACHE_PERIOD = -1
 _USE_FILE_CACHE = False
 DEFAULT_EXT_DIRECTORY = None
 
-_EXTENSIONS: Dict[str, "IqmoQlExtension"] = {}
-_DBCONNECTOR: Optional["DatabaseConnector"] = None
+# DB_MODULE is loaded on first call to get_dbmodule()
+# Replace this string with another connector prior to first use,
+# or set _DBCONNECTOR to None after changing.
+DB_MODULE: str = "iql.db_connectors.duckdb_connector"
+
+_EXTENSIONS: Dict[Tuple[str, str], "IqlExtension"] = {}
+_DBCONNECTOR: Optional["IqlDatabaseConnector"] = None
 
-# Used internally to name the dataframes registered with duckdb
-_DFPREFIX: str = "iqmodf"
+# Used internally to name the dataframes
+_DFPREFIX: str = "iqldf"
 
 # Add extensions via register_extension()
 # Extensions are loaded on first access, to avoid requiring
 # unused dependencies
 _KNOWN_EXTENSIONS: Dict[str, str] = {
     "bql": "iql.bbg_bql.bql_extension",
     "s3": "iql.extensions.aws_s3_extension",
     "fred": "iql.extensions.fred_extension",
     "kaggle": "iql.extensions.kaggle_extension",
     "edgar": "iql.extensions.edgar_extension",
     "pandas": "iql.extensions.pandas_extension",
 }
 
+_ALIASES: Dict[str, str] = {}
+
 logger = logging.getLogger(__name__)
 
 
-class DatabaseConnector:
+def _find_closing_paren(text: str, start: int) -> int:
+    # TODO: Handle escaping
+    paren_depth = 1
+    quote_stack = []
+    for i in range(start, len(text)):
+        c = text[i]
+        if c == "(" and len(quote_stack) == 0:
+            paren_depth += 1
+        elif c == "'" or c == '"':
+            if len(quote_stack) == 0:
+                quote_stack.append(c)
+            elif quote_stack[len(quote_stack) - 1] == c:
+                quote_stack.remove(c)
+        elif c == ")" and len(quote_stack) == 0:
+            paren_depth -= 1
+
+        if paren_depth == 0:
+            end = i
+            return end
+    raise ValueError("Never found closing parenthesis, probably unbalanced query")
+
+
+def get_keyword_list(keywords: Optional[List[str]] = None) -> str:
+    if keywords is None:
+        keywords = list(_KNOWN_EXTENSIONS.keys())
+    _keyword_list = "|".join((k if isinstance(k, str) else k[0] for k in keywords))
+    return _keyword_list
+
+
+def _extract_subquery_strings(
+    query, keywords: Optional[List[str]] = None
+) -> List[Tuple[str, str, str, str]]:
+    global _cached_pats
+    """Finds the subqueries start with keyword, along with matching end paren
+    keyword(....)
+    keyword.subword(....)
+    """
+    _keyword_list = get_keyword_list(keywords)
+
+    _kpat = re.compile(rf"(?s)({_keyword_list})(\.(\w+))?\s*\(")
+
+    results = []
+    for m in re.finditer(_kpat, query):
+        keyword = m.group(1)
+        subword = m.group(3)
+        paren_start = m.end()  # just after the last paren
+
+        paren_end = _find_closing_paren(query, paren_start)
+
+        outer = query[m.start() : paren_end + 1]
+        inner = query[paren_start : paren_end + 1]
+        logger.debug(
+            f"Extracted subquery: {keyword}.{subword} at {paren_start}:{paren_end}"
+        )
+
+        results.append((keyword, subword, outer, inner))
+
+    return results
+
+
+def rename_dupe_arrow_columns(pat: Table) -> Table:
+    # PyArrow can't export to Pandas if there are duplicate columns
+    cols = pat.column_names
+    unique_cols = set(cols)
+
+    if len(unique_cols) == len(cols):
+        # everything is unique
+        return pat
+    else:
+        newcols = []
+        print(f"Has dupes, {cols}")
+        seen = set()
+        for col in cols:
+            if col not in seen:
+                seen.add(col)
+                newcols.append(col)
+            else:
+                idx = 1
+                while (newcol := f"{col}_{idx}") in seen or newcol in unique_cols:
+                    idx += 1
+                newcols.append(newcol)
+
+        pat = pat.rename_columns(newcols)
+
+        return pat
+
+
+@dataclass
+class IqlResult:
+    _table: Table
+
+    def arrow(self):
+        return self._table
+
+    def df_numpy(self):
+        return self._table.to_pandas()
+
+    def df_arrow(self):
+        return self._table.to_pandas(types_mapper=pd.ArrowDtype)
+
+
+class IqlDatabase:
     @abstractmethod
     def execute_query(
-        self, con: object, query: str, completed_dfs: Dict[str, DataFrame]
-    ) -> List[DataFrame]:
+        self, query: str, completed_dfs: Dict[str, DataFrame]
+    ) -> Optional[IqlResult]:
         raise ValueError("Implement Me")
 
     @abstractmethod
     def get_connection(self) -> object:
         raise ValueError("Implement Me")
 
     @abstractmethod
-    def close_connection(self, con):
+    def close_db(self):
+        raise ValueError("Implement Me")
+
+
+class IqlDatabaseConnector:
+    @abstractmethod
+    def create_database(self) -> IqlDatabase:
+        raise ValueError("Implement Me")
+
+    @abstractmethod
+    def create_database_from_con(self, con: object) -> IqlDatabase:
         raise ValueError("Implement Me")
 
 
 _lasttoken = None
 
 
+def get_subqueries_flat(queries: List["SubQuery"]) -> List["SubQuery"]:
+    subqueries_flat = [
+        q_inner for q_outer in queries for q_inner in q_outer.get_subqueries_flat()
+    ]
+    return subqueries_flat
+
+
 @dataclass
-class IqmoQlExtension:
+class IqlExtension:
     keyword: str
+    subword: str = field(default=None, init=True)  # type: ignore
+
+    # Extensions must be parallelizable, or must
+    # implement their own execute_batch.
+    # Can only contain pickleable elements
+    # etc
 
     # Determines whether the local cache settings should be used
     # vs  CACHE_PERIOD and
     # USE_FILE_CACHE
     use_default_caching: bool = field(default=True, init=False)
     _cache_period: Optional[int] = field(default=None, init=False)
     _use_file_cache: bool = field(default=False, init=False)
-
     temp_file_directory: Optional[str] = field(default=None, init=False)
 
-    def allow_cache_read_inner(self, sq: "SubQuery") -> bool:
-        """Dont use cached values if nocache=True. Used by individual externals for internal caching."""
-        if sq.options.get("nocache") is True:
-            return False
-        else:
-            return True
+    def get_output_dir(self) -> str:
+        tempdir = (
+            self.temp_file_directory if self.temp_file_directory is not None else "./"
+        )
+        return tempdir
 
     def allow_cache_read(self, sq: "SubQuery") -> bool:
         """Dont use cached values"""
         if sq.options.get("nocache") is True:
             return False
         elif sq.options.get("cache") is not None:
             return True
@@ -114,89 +238,148 @@
         if self.use_default_caching:
             return _USE_FILE_CACHE
         else:
             return self._use_file_cache
 
     def use_path_replacement(self) -> bool:
         """Some extensions just return a filestring to use instead of the SubQuery, such as the
-        S3 Extension. If execute() returns None, then use_path_replacement must be used."""
+        S3 Extension. If execute() returns None, then use_path_replacement must be used.
+        """
         return False
 
-    def get_path_replacement(self, query: str) -> Optional[str]:
+    def get_path_replacement(
+        self, subquery: "SubQuery", quote: bool = True
+    ) -> Optional[str]:
+        """Quoting is done here, with the expectation that some path replacements might actually be function calls."""
+        tempdir = self.get_output_dir()
+        filepath = f"{tempdir}/{subquery.name}.parquet"
+
+        if quote:
+            outpath = f"'{filepath}'"
+        else:
+            outpath = filepath
+
+        logger.info(f"Converted {subquery} to {outpath}")
+        return outpath
+
         """Used for extensions which use a native duckdb extension to access the underlying data"""
         return None
 
     @abstractmethod
     def executeimpl(self, sq: "SubQuery") -> Optional[DataFrame]:
         raise ValueError("Implement Me")
 
     def execute(self, sq: "SubQuery") -> Optional[DataFrame]:
         # usage: select * from (verityapi(functionname, targetname)) as verityquery
         # An empty response means no response was needed
         # Internal failure must raise an exception
         if sq.populate_from_cache() and sq.dataframe is not None:
             return sq.dataframe
 
-        logger.debug(f"Executing query {sq.get_query()}")
+        logger.debug(f"Executing query {sq.subquery}")
 
         df = self.executeimpl(sq)
 
         if df is None and not self.use_path_replacement():
             raise ValueError("Empty DF, should never reach here")
         else:
             if df is not None:
                 pivot_options = sq.options.get("pivot")
+                melt_options = sq.options.get("melt")
 
                 df = self.apply_pandas_operations_prepivot(df, sq.options)
 
                 if pivot_options is not None:
                     df = self.pivot(df, pivot_options)  # type: ignore
+                if melt_options is not None:
+                    df = df.melt(melt_options)
+
                 df = self.apply_pandas_operations_postpivot(df, sq.options)
 
                 sq.dataframe = df
 
                 sq.save_to_cache()
 
                 return df
 
     def execute_batch(self, queries: List["SubQuery"]) -> Dict[str, DataFrame]:
         """Default implementation runs individually, override for functions that can be batched, such as
-        BQL's _many functions"""
+        BQL's _many functions.
+        Executes all subqueries first, then merges as required.
+        SubQueries are executed in a threadpool, which has minimal benefit."""
+
+        completed_dfs = {}
+        # context = get_context('spawn')
+
+        subqueries_flat = get_subqueries_flat(queries)
+        # Get all the queries (and any queries inside SubQueryGroups)
+
+        # Executes the ungrouped queries
+
+        if te.ENABLED and te.MAX_PROCESSES > 1 and len(queries) > 1:
+            te.execute_batch(subqueries_flat, self.execute)
+        else:
+            for query in subqueries_flat:
+                self.execute(query)  # type: ignore
 
         completed_dfs = {}
+        # Merge the results
         for query in queries:
-            df = self.execute(query)  # type: ignore
+            # For single subqueries, this is a noop
+            # For subquery groups, this merges the results of the children
+            query.merge()
+
+            df = query.dataframe
             if df is None and not self.use_path_replacement():
                 raise ValueError(f"Empty DF, {query.get_query()} failed")
             elif df is None:
                 logger.debug("Using path replacement, no DF")
             else:
                 query.dataframe = df  # type: ignore
                 completed_dfs[query.name] = df
 
         return completed_dfs
 
-    def create_subqueries(self, query: str, name: str, con: object) -> List["SubQuery"]:
+    def create_subquery(
+        self, subquery: str, name: str, iqc: "IqlQueryContainer"
+    ) -> "SubQuery":
+        logger.debug("Creating subquery")
+        sq = SubQuery(extension=self, subquery=subquery, name=name, iqc=iqc)
+        return sq
+
+    def create_subqueries(
+        self,
+        query: str,
+        name: str,
+        iqc: "IqlQueryContainer",
+        create_function: Optional[Callable] = None,
+    ) -> List["SubQuery"]:
+        """Converted to always return a single item, but left logic in place to support multiple"""
         logger.debug(f"Creating a subquery {name} for {query}")
 
-        sq = SubQuery(extension=self, subquery=query, name=name, dbcon=con)
+        if create_function is None:
+            create_function = self.create_subquery
+
+        sq = create_function(subquery=query, name=name, iqc=iqc)
 
         # If a paramlist is passed, create one subquery for each value
 
         if "paramquery" in sq.options:
             paramquery: Tuple[str, str] = sq.options.get("paramquery")  # type: ignore
 
             if (
                 len(paramquery) == 2
                 and isinstance(paramquery[0], str)
                 and isinstance(paramquery[1], str)
             ):
                 parameter_name = paramquery[0]
                 param_query = paramquery[1]
-                df = con.sql(param_query).to_df()  # type: ignore
+                result = iqc.db.execute_query(param_query, completed_dfs={})  # type: ignore
+
+                df = result.df_numpy()
                 parameter_values = df[df.columns[0]].values
                 logger.debug(f"Values {parameter_values}")
             else:
                 raise ValueError(f"Invalid options passed to paramquery: {paramquery}")
 
         elif "paramlist" in sq.options:
             paramlist: Tuple[str, List[str]] = sq.options.get("paramlist")  # type: ignore
@@ -214,28 +397,37 @@
             if isinstance(parameter_values, str):
                 parameter_values = [parameter_values]
         else:
             parameter_name = None
             parameter_values = None  # type: ignore
 
         if parameter_name is not None:
-            assert parameter_values is not None
+            assert parameter_values is not None and len(parameter_values) > 0
             sqs: List["SubQuery"] = []
             count = 1
 
             for v in parameter_values:
                 v_query = query.replace(parameter_name, v)
 
-                sq = SubQuery(
-                    extension=self, subquery=v_query, name=f"{name}_{count}", dbcon=con
+                sq = create_function(  # type: ignore
+                    subquery=v_query, name=f"{name}_{count}", iqc=iqc
                 )
+
                 sqs.append(sq)
                 count += 1
 
-            return sqs
+            sq_group = SubQueryGroup(
+                subqueries=sqs,
+                extension=self,
+                subquery=name,  # subqueries are ignored for subquerygroups
+                name=f"{name}_group",
+                iqc=iqc,
+            )
+
+            return [sq_group]
         else:
             return [sq]
 
     def fix_col_ref(self, opt: str, columns: List[str]):
         if opt in columns:
             return opt
         opt_l = opt.lower().strip()
@@ -262,15 +454,14 @@
             working_df = working_df.dropna(subset=dropna_opt)
 
         return working_df
 
     def apply_pandas_operations_prepivot(
         self, working_df, options: Dict[str, object]
     ) -> DataFrame:
-
         # only drops from the "value" column
         fillna_opt: str = options.get("fillna_pre")  # type: ignore
         if fillna_opt is not None:
             logger.debug(f"Filling NaNs with in value column with {fillna_opt}")
             working_df["value"] = working_df["value"].fillna(fillna_opt)
 
         dropna_opt = options.get("dropna_pre")
@@ -386,15 +577,20 @@
                     index=index,
                     columns=column,
                     values=value,
                 )
 
         working_df = working_df.reset_index()
 
-        if isinstance(column, list) and len(column) > 1:
+        if isinstance(value, list) and len(value) > 1:
+            working_df.columns = [
+                "_".join(reversed(str(col) if type(col) == int else col))
+                for col in working_df.columns.values
+            ]
+        elif isinstance(column, list) and len(column) > 1:
             # Flatten multicolumn indices
             working_df.columns = [
                 "_".join(str(col) if type(col) == int else col)
                 for col in working_df.columns.values
             ]
 
         # Clean columns
@@ -419,35 +615,47 @@
             working_df = working_df.rename(columns=renames)
 
         return working_df
 
 
 @dataclass
 class SubQuery:
-    extension: IqmoQlExtension
+    extension: IqlExtension
     subquery: str
     name: str
-    dbcon: object
+    iqc: "IqlQueryContainer"
     dataframe: Optional[DataFrame] = field(default=None, init=False)
 
     options: Dict[str, object] = field(default_factory=dict, init=False)
+    input_data: object = field(default=None, init=False)
+
+    local_dfs: Dict[str, object] = field(default_factory=dict, init=False)
+
+    def get_subqueries_flat(self) -> List["SubQuery"]:
+        return [self]
+
+    def merge(self):
+        # Nothing to do for a single subquery
+        pass
 
     def get_query(self) -> str:
         """Returns the first parameter to:
         keyword(query, *params)"""
         if len(self.options) == 0:
-            raise ValueError("Options not properly passed or parsed")
+            raise ValueError(f"Options not properly passed or parsed ({self.subquery})")
 
         query = next(iter(self.options.keys()))
         return query
 
     def __post_init__(self):
-        logger.debug(f"Parsing subquery for {self.subquery}")
-        self.options: Dict[str, object] = options_parser.options_to_list(self.subquery)
-        logger.debug(f"Options: {self.options}")
+        if self.subquery is not None:
+            self.options: Dict[str, object] = options_parser.options_to_list(
+                self.subquery
+            )
+            logger.debug(f"Options: {self.options}")
 
     def populate_from_cache(self) -> bool:
         """Returns cached value if it's available"""
         cache_val = self.subquery
 
         logger.debug(f"Checking cache for {cache_val}, {type(self)}")
         if not self.extension.allow_cache_read(self):
@@ -486,289 +694,345 @@
                 key=cache_val,
                 o=self.dataframe,
                 duration_seconds=cache_period,
                 use_file_cache=self.extension.use_file_cache(),
             )
 
 
-class IqmoQueryContainer:
-    # This is used so we can run the bql_queries as an async batch, separate from processing the results.
-    orig_query: str
-    query: str
+@dataclass
+class SubQueryGroup(SubQuery):
+    """SubQueryGroups represent a set of queries whose outputs will be combined.
+    SubQueries are executed in parallel (via get_subqueries_flat),
+    so this step is needed to gather the results.
+
+    Our first implementation was to rely on database Unions, but performance wasn't
+    great.
+
+    Future: SubQueryGroups could support nesting, only one level supported now."""
+
     subqueries: List[SubQuery]
-    con: object
 
-    def _extract_replacements(self) -> List[SubQuery]:
-        """Extensions are functions within the SQL, which will be replaced by dataframes
-        Example - assuming bql is a registered extension:
-            select * from bql("....") as q1
-        will be replaced with:
-            select * from df1 as q1
+    def __post_init__(self):
+        self.subquery = None  # type: ignore
+        self.options = None  # type: ignore
 
-        And "bql("....")" will be executed via the bql_extension.
+    def get_subqueries_flat(self) -> List[SubQuery]:
+        return self.subqueries
 
-        Returns: ( modified_query , Dict[name, Subquery] )
+    def get_query(self) -> str:
+        raise ValueError("SubQueryGroups do not have a query")
+
+    def merge(self):
+        """Since each file may have a different schema, we'll read them all and let's Pandas concat
+        sort it out. Using DuckDb "union by name" ran into an error (hash table memory)
         """
 
-        extension_keywords = list_extensions()
+        if self.extension.use_path_replacement():
+            files = [
+                self.extension.get_path_replacement(sq, quote=False)
+                for sq in self.subqueries
+            ]
+
+            logger.info(f"Read {len(files)} parquet files")
 
-        if len(extension_keywords) == 0:
-            raise ValueError("No EXTENSIONS defined")
+            dfs = [pd.read_parquet(f) for f in files]
+            logger.info("Done reading, concatting")
 
-        # remove comments from query
-        query = self.query
-        query = sqlparse.format(query, strip_comments=True).strip()
+            df = pd.concat(dfs)
 
-        replacements: Dict[str, str] = {}
+            outfile = self.extension.get_path_replacement(self, quote=False)
+            logger.info(f"Writing to final parquet file {outfile}")
+
+            df.to_parquet(outfile)
+
+        else:
+            dfs: List[DataFrame] = [sq.dataframe for sq in self.subqueries]  # type: ignore
+            logger.debug(f"Concatting {len(dfs)}")
+            self.dataframe = pd.concat(dfs)
+
+        logger.info(f"Done merging {len(self.subqueries)} subqueries")
+
+
+class IqlQueryContainer:
+    # This is used so we can run the bql_queries as an async batch, separate from processing the results.
+    orig_query: str
+    query: str
+    subqueries: List[SubQuery]
+    db: Optional[object]
+
+    def extract_subqueries(self):
         subqueries: List[SubQuery] = []
 
-        def process_node(token, level: int = 0):
-            global last_real_name
-            real_name = token.get_real_name()
-            this_last_real_name = last_real_name
-            last_real_name = real_name
-            # alias = token.get_alias()
-            value = token.value
-            useThis = False
-            name = f"{_DFPREFIX}{len(replacements) + 1}"
-            if (
-                real_name is None
-                and type(token) == sqlparse.sql.Parenthesis
-                and this_last_real_name in extension_keywords
-            ):
-                if re.match(rf"(?s)[\(\s]+{real_name}.*", value) is not None:
-                    # WITH alias as bql(....)
-                    useThis = True
-                    logger.debug(
-                        "real name is None, but we're in a paren and last_real_name was a keyword"
-                    )
+        i = 0
 
-            if real_name in extension_keywords or useThis:
+        replacements: Dict[str, Optional[str]] = {}
 
-                if real_name is None and this_last_real_name in extension_keywords:
-                    real_name = this_last_real_name
-                    value = f"{real_name}{value}"
-
-                # remove the prefix (abc as ...), for WITHs
-                value = value[value.index(real_name) :]
-                # remove any suffix (...) as abc, for SELECTs
-                if ")" in value:
-                    value = value[: value.rindex(")") + 1]
-
-                logger.debug(f"Found extension {real_name}, value: {value}")
-                global _lasttoken
-                _lasttoken = token
-                if str(real_name.strip()) == str(
-                    value.strip()
-                ):  # in some cases, the () section is parsed as the next token
-                    logger.debug("Skip this, the next paren is what we need")
-                    return
-
-                extension = get_extension(real_name)
-
-                sqs: List[SubQuery] = extension.create_subqueries(value, name, self.con)
-
-                subqueries.extend(sqs)
-
-                if extension.use_path_replacement():
-                    names = [
-                        sq.extension.get_path_replacement(sq.get_query()) for sq in sqs
-                    ]
-                else:
-                    names = [sq.name for sq in sqs]
+        if "--" in self.orig_query:
+            query = sqlparse.format(self.orig_query, strip_comments=True).strip()
+        else:
+            query = self.orig_query
+
+        for keyword, subword, outer, inner in _extract_subquery_strings(query):
+            i += 1
+            name = f"{_DFPREFIX}_{i}"
+
+            extension = get_extension(keyword, subword)
+            sqs: List[SubQuery] = extension.create_subqueries(
+                query=outer, name=name, iqc=self
+            )
+            subqueries.extend(sqs)
 
+            if extension.use_path_replacement():
+                names = [sq.extension.get_path_replacement(sq) for sq in sqs]
+            else:
+                names = [sq.name for sq in sqs]
+
+            if len(names) == 1:
+                result = names[0]
+            else:
                 querystrings = [f"(select * from {i})" for i in names]
-                if len(querystrings) == 1:
-                    result = querystrings[0]
-                else:
-                    # SQL Union of the results
-                    # '((select * from a) union (select * from b) union (select * from c))'
-                    result = " union ".join(querystrings)
-                    result = f"({result})"
-
-                replacements[value] = result
-
-                return
-            for t in token.get_sublists():
-                process_node(t, level + 1)
 
-        for s in sqlparse.parse(query):
-            process_node(s)
+                result = " UNION ".join(querystrings)
+                result = f"({result})"
+
+            replacements[outer] = result
 
         for old, new in replacements.items():
-            query = query.replace(old, new)
+            logger.debug(f"Replacing {old} with {new}")
+            query = query.replace(old, new)  # type: ignore
+
+        # if only one function without a beginning subquery
+        if len(replacements) > 0:
+            values = [value for value in replacements.values() if value is not None]
+            if re.match(rf"(?s)\s*({'|'.join(values)}).*", query) is not None:
+                logger.info(f"Starts with replacement {values}")
+                query = f"select * from {query}"
 
         self.query = query
 
-        logger.debug(self.query)
         return subqueries
 
-    def __init__(self, query: str, con: Optional[object]):
+    def __init__(self, query: str, db: IqlDatabase):
         self.orig_query = query
         self.query = query
-        self.con = con
+        self.db = db
 
-        self.subqueries = self._extract_replacements()
+        self.subqueries = self.extract_subqueries()
+        # self.subqueries = self._extract_replacements()
         # Sanity checks. These don't take into account escaping or quoting, so they're just warnings.
         if query.count("(") != query.count(")"):
             logger.warning("Left and Right Paren counts aren't equal")
 
         if query.count("'") % 2 != 0:
             logger.warning("Uneven number of single quotes")
 
         if query.count('"') % 2 != 0:
             logger.warning("Uneven number of double quotes")
 
-    def get_subqueries_by_extension(self, keyword: str) -> List[SubQuery]:
+    def get_subqueries_by_extension(self, keyword: str, subword: str) -> List[SubQuery]:
         results: List[SubQuery] = []
-        results = [s for s in self.subqueries if s.extension.keyword == keyword]
+        results = [
+            s
+            for s in self.subqueries
+            if s.extension.keyword == keyword and s.extension.subword == subword
+        ]
 
         return results
 
-    def execute(self) -> List[DataFrame]:
+    def execute(self) -> Tuple[Optional[DataFrame], List[DataFrame]]:
+        """Returns the final df, plus the intermediate subquery dataframes.
+        If the query is not a Select, returns a None"""
         # Execute the subqueries
-        if _DBCONNECTOR is None:
-            raise ValueError("DBConnector Not Set")
 
-        if self.con is None:
-            con = _DBCONNECTOR.get_connection()
-        else:
-            con = self.con
-        try:
-            completed_dfs: Dict[str, DataFrame] = {}
+        completed_dfs: Dict[str, DataFrame] = {}
 
-            for keyword, e in _EXTENSIONS.items():
-                # db_connection is used by Pandas extension
-                # TODO: This isn't thread safe, since extensions are reused
+        for (keyword, subword), e in _EXTENSIONS.items():
+            sqs: List[SubQuery] = self.get_subqueries_by_extension(keyword, subword)  # type: ignore
 
-                sqs: List[SubQuery] = self.get_subqueries_by_extension(keyword)
-                e_dfs = e.execute_batch(sqs)
+            e_dfs = e.execute_batch(sqs)  # type: ignore
 
-                completed_dfs.update(e_dfs)
+            for k, df in e_dfs.items():
+                if df is not None:
+                    completed_dfs[k] = df
 
-            return _DBCONNECTOR.execute_query(
-                con=con, query=self.query, completed_dfs=completed_dfs
-            )
-        finally:
-            if self.con is None:
-                # If connection is created in this function
-                con.close()  # type: ignore
+        result = self.db.execute_query(query=self.query, completed_dfs=completed_dfs)  # type: ignore
+        df = result.df_numpy()
 
+        return (df, completed_dfs)  # type: ignore
 
-def execute(
-    query: str, keyword: Optional[str] = None, con: Optional[object] = None
-) -> Optional[DataFrame]:
-    """Executes the given SQL query. Keyword is only used to run a single subquery without SQL."""
 
-    fthree = query.strip(" \t\n\r").lower()[0:3]
-    if fthree in ["let", "get"]:
-        keyword = "bql"
-
-    if keyword is not None:
-        # Special convenience case if you're running just a single subquery
-        query = escaped = query.replace(
-            '"', '\\"'
-        )  # not perfect, doesn't handled escaped
-        query = f'{keyword}("{escaped}")'
+class IqlPlan:
+    pass
+
+
+def _parameterize_sql_alias(subword, query) -> str:
+    if subword not in _ALIASES.keys():
+        raise ValueError(f"Unknown alias {subword}")
+
+    base_query = _ALIASES[subword]
+
+    for k, v in options_parser.options_to_list(query).items():
+        # convert the parameter to $uppercase, so security => $SECURITY
+        newk = f"${k.upper()}"
+        if newk not in base_query:
+            raise ValueError(f"Parameter {k} / {newk} not in alias SQL")
+        else:
+            base_query = base_query.replace(newk, str(v))
+
+    return base_query
+
+
+def replace_sql_aliases(query) -> str:
+    newquery = query
+    for keyword, subword, outer, inner in _extract_subquery_strings(query, ["alias"]):
+        sql = _parameterize_sql_alias(subword, outer)
+
+        logger.debug(f"Found SQL alias, replacing and parameterizing: {outer}")
+
+        newquery = newquery.replace(outer, sql)
+        # logger.info(f"After alias replacement {query}")
 
-    # If passed a connection, don't close it.
-    close_connection = con is None
+    return newquery
 
+
+def execute_full_results(
+    query: str, con: Optional[object] = None
+) -> Tuple[Optional[DataFrame], Optional[List[DataFrame]], IqlPlan]:
+    # Connection to database
+    get_dbconnector()
+    if _DBCONNECTOR is None:
+        raise ValueError("DBConnector Not Set")
     if con is None:
-        get_dbconnector()
+        db = _DBCONNECTOR.create_database()
+    else:
+        db = _DBCONNECTOR.create_database_from_con(con=con)
 
-        if _DBCONNECTOR is None:
-            raise ValueError("DBConnector Not Set")
+    # Aliases
+    query = replace_sql_aliases(query)
 
-        con = _DBCONNECTOR.get_connection()
+    # Placeholder for an IqlPlan (noop for now)
+    iqlplan: IqlPlan = IqlPlan()
 
     try:
-        dfs = None
         # A single query might contain multiple SQL statements. Parse them out and iterate:
-        for statement in sqlparse.parse(query):
-            singlequery = statement.value.strip(";")
-            iqc = IqmoQueryContainer(query=singlequery, con=con)
 
-            # Run each statement, but only keep the results from the last one
-            dfs = iqc.execute()
+        df = None
+        completed_dfs = None
+        if ";" not in query:
+            # Performance optimization for simple queries
+            iqc = IqlQueryContainer(query=query, db=db)
+
+            df, completed_dfs = iqc.execute()
+        else:
+            for statement in sqlparse.parse(query):
+                singlequery = statement.value.strip(";")
+                iqc = IqlQueryContainer(query=singlequery, db=db)
+
+                # Run each statement, but only keep the results from the last one
+                df, completed_dfs = iqc.execute()
 
         # The first result is the query result. The other df's are for debugging purposes
         # If it's not a select, there won't be response, such as in a COPY (..) TO
 
-        if dfs is None:
-            return None
-
-        return dfs[0] if len(dfs) > 0 else None
+        return (df, completed_dfs, iqlplan)
 
     finally:
-        if close_connection:
+        if con is None:  # DB was created here, so close it
+            db.close_db()
 
-            if _DBCONNECTOR is None:
-                raise ValueError("DBConnector Not Set")
 
-            _DBCONNECTOR.close_connection(con)
+def execute(query: str, con: Optional[object] = None) -> Optional[DataFrame]:
+    """Executes the given SQL query. Keyword is only used to run a single subquery without SQL."""
+
+    if query.strip().startswith("get") or query.strip().startswith("let"):
+        query = query.replace('"', '"')
+        query = f"""select * from bql("{query}")"""
+    df, completed_dfs, iql_plan = execute_full_results(query, con)
 
+    return df
 
-def get_dbconnector() -> DatabaseConnector:
+
+def get_dbconnector() -> IqlDatabaseConnector:
     global _DBCONNECTOR
     if _DBCONNECTOR is None:
         # Initializes only on first reference
         module = importlib.import_module(DB_MODULE)
         _DBCONNECTOR = module.getConnector()
 
     if _DBCONNECTOR is None:
         raise ValueError("Failure initializing _DBCONNECTOR")
     return _DBCONNECTOR
 
 
-def register_extension(e: IqmoQlExtension):
-    _EXTENSIONS[e.keyword] = e
+def register_extension(e: IqlExtension):
+    _EXTENSIONS[(e.keyword, e.subword)] = e  # type: ignore
     if e.keyword not in _KNOWN_EXTENSIONS.keys():
         _KNOWN_EXTENSIONS[e.keyword] = e.keyword
 
     if e.temp_file_directory is None:
         e.temp_file_directory = DEFAULT_EXT_DIRECTORY
 
 
+def register_alias(subword: str, sql: str):
+    """
+    Aliases are called via
+    alias.aliasname(param1=abc, param2.abc)
+    When run, the alias will be replaced, and "$PARAM1" will be replaced with abc
+    """
+    logger.debug(f"Registering alias: {subword}")
+    _ALIASES[subword] = sql
+
+
 def list_extensions() -> List[str]:
     return list(_KNOWN_EXTENSIONS.keys())
 
 
-def get_extension(keyword: str) -> "IqmoQlExtension":
+def get_extension(keyword: str, subword: str) -> "IqlExtension":
     """Loads extension on first use"""
-    if keyword in _EXTENSIONS:
-        return _EXTENSIONS[keyword]
+
+    words = (keyword, subword)
+    if words in _EXTENSIONS:
+        return _EXTENSIONS[words]
     elif keyword not in _KNOWN_EXTENSIONS.keys():
         raise ValueError(f"Unknown Extension {keyword}")
     else:
         # Dynamically load extensions on first use
         # This avoids requiring installation of packages that
         # aren't needed
         classname = _KNOWN_EXTENSIONS[keyword]
         module = importlib.import_module(classname)
         module.register(keyword)
 
-        return _EXTENSIONS[keyword]
+        if words not in _EXTENSIONS:
+            raise ValueError(f"{keyword}.{subword} is not registered")
+        return _EXTENSIONS[words]
 
 
-def activate_cache(
-    duration_seconds: Optional[int] = -1, cache_directory: Optional[str] = None
+def configure(
+    duration_seconds: Optional[int] = -1,
+    cache_directory: Optional[str] = None,
+    temp_dir: Optional[str] = None,
+    max_processes: Optional[int] = None,
 ):
     """
     Must be called before extensions are initialized (on first use)
     duration_seconds: None (Disabled), -1 (Infinite), int (Seconds)
     file_directory: None (no file cache), string (output directory)
     """
     global _CACHE_PERIOD
     global _USE_FILE_CACHE
-    global _DEFAULT_EXT_DIRECTORY
+    global DEFAULT_EXT_DIRECTORY
 
     _CACHE_PERIOD = duration_seconds
     if cache_directory is None:
         _USE_FILE_CACHE = False
     else:
         _USE_FILE_CACHE = True
         if not os.path.exists(cache_directory):
             raise ValueError(f"cache_directory {cache_directory} does not exist")
 
-        _DEFAULT_EXT_DIRECTORY = cache_directory
         qc.activate_file_cache(cache_directory)
+
+    DEFAULT_EXT_DIRECTORY = temp_dir
+
+    if max_processes is not None:
+        te.MAX_PROCESSES = max_processes
```

## iql/options_parser.py

```diff
@@ -19,37 +19,37 @@
             val = convert(e)
             v.append(val)
         return v
     elif isinstance(node, ast.Str):
         return node.s
     elif isinstance(node, ast.Constant) or isinstance(node, ast.NameConstant):
         return node.value
+    elif isinstance(node, ast.Num):
+        return node.n
     else:
         return node.id
 
 
 def options_to_list(options: str) -> Dict[str, object]:
     logger.debug(f"Analyzing {options}")
     options = options.replace("\n", " ")
     p = ast.parse(options)
 
     results = {}
 
     for e in p.body:
-
         if isinstance(e.value, ast.Name):  # type: ignore
             results[e.value] = None  # type: ignore
 
             continue
         else:
             for arg in e.value.args:  # type: ignore
                 results[arg.s] = None
 
         for k in e.value.keywords:  # type: ignore
-
             r = convert(k.value)
 
             results[k.arg] = r
 
             continue
 
     return results
```

## iql/q_cache.py

```diff
@@ -18,15 +18,14 @@
 _MEMCACHE: Dict[str, Tuple[Optional[float], object]] = {}
 
 # FCACHE must be activated prior to use
 _FCACHE: Optional[Dict[str, Tuple[Optional[float], object]]] = None
 
 
 def _get_cache(use_file_cache: bool) -> Dict[str, Tuple[Optional[float], object]]:
-
     if use_file_cache:
         if _FCACHE is None:
             logger.debug(
                 "File cache selected but file cache not activated, using mem cache instead"
             )
             cache = _MEMCACHE
         else:
@@ -44,64 +43,66 @@
 def save(
     key: str,
     o: object,
     duration_seconds: Optional[int] = None,
     use_file_cache: bool = False,
     type: str = "default",
 ):
-
     if duration_seconds is None:
         logger.debug(f"No caching {key}")
+        raise ValueError("test")
         return
 
-    key = _str_to_key(key)
+    actualkey = _str_to_key(key)
+    logger.debug(f"Saving {actualkey} for {key} for duration {duration_seconds}")
+
     if duration_seconds == -1:
         # Infinite Cache
         expiration = None
     else:
         expiration = time.time() + duration_seconds
 
     cache = _get_cache(use_file_cache)
-    cache[key] = (expiration, o)
+    cache[actualkey] = (expiration, o)
 
 
 def get(key: str, use_file_cache: bool = False) -> object:
-    key = _str_to_key(key)
+    logger.debug(f"Getting {key}")
+
+    actualkey = _str_to_key(key)
     cache = _get_cache(use_file_cache)
 
-    if key not in cache:
-        logger.debug(f"Not in cache: {key}")
+    if actualkey not in cache:
+        logger.debug(f"Not in cache: {actualkey} for {key}")
         return None
     else:
-        logger.debug(f"In cache: {key}")
-
-        expiration, o = cache[key]
+        logger.debug(f"In cache: {actualkey} for {key}")
 
+        expiration, o = cache[actualkey]
         if expiration is not None and time.time() > expiration:
-            del cache[key]
+            del cache[actualkey]
             return None
         else:
             return o
 
 
 def clear(key: str):
-    logger.debug(f"Clearing from cache: {key}")
-
-    key = _str_to_key(key)
+    actualkey = _str_to_key(key)
+    logger.debug(f"Clearing from cache: {actualkey} for {key}")
 
     try:
-        del _MEMCACHE[key]
+        del _MEMCACHE[actualkey]
     except Exception:
-        logger.debug(f"Del failed, not in mcache: {key}")
+        logger.debug(f"Del failed, not in mcache: {actualkey} for {key}")
 
     if _FCACHE is not None:
         try:
-            del _FCACHE[key]
+            del _FCACHE[actualkey]
         except Exception:
-            logger.debug(f"Del failed, not in fcache: {key}")
+            logger.debug(f"Del failed, not in fcache: {actualkey} for {key}")
 
 
 def clear_caches():
     global _MEMCACHE, _FCACHE
 
     _MEMCACHE = {}
     if _FCACHE is None:
```

## iql/bbg_bql/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-# Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
-# All Rights Reserved
+# Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
+# All Rights Reserved
```

## iql/bbg_bql/bql_datamodel.py

```diff
@@ -92,15 +92,14 @@
         default_factory=dict
     )  # parameters. Convention is $FIELD: value
 
     def get_fields(self) -> List[str]:
         return self.fields
 
     def to_bql_query(self) -> str:
-
         for_str_mod = security_to_finalstr(self.for_str)
 
         if SECURITY_KEYWORD not in self.params and self.security is not None:
             self.params[SECURITY_KEYWORD] = self.security
 
         sec = self.params.get(SECURITY_KEYWORD)
         if self.let_str is not None and sec is not None:
@@ -110,26 +109,25 @@
         query_str = construct_bql_query(
             self.fields, for_str_mod, self.with_params, let_str_mod
         )
 
         logger.debug(f"After construction but before replacement: {query_str}")
         for param, value in self.params.items():
             if param == SECURITY_KEYWORD:
-
                 if isinstance(value, str) and (
                     "'" in self.for_str or "(" in self.for_str or "[" in self.for_str
                 ):
                     # Don't change anything if security is a list, or the for_str is a formula
                     pass
                 else:
                     value = security_to_finalstr(self.params[SECURITY_KEYWORD])
 
             query_str = query_str.replace(param, value)
 
-        logger.info(f"BQL Query to String: {query_str}")
+        logger.debug(f"BQL Query to String: {query_str}")
         return query_str
 
 
 class DateGen:
     start_date: str
     end_date: str
     date_param: str
@@ -141,15 +139,14 @@
     def __init__(self, date_param, start_date, end_date, date_frequency="MS"):
         self.date_param = date_param
         self.start_date = start_date
         self.end_date = end_date
         self.date_frequency = date_frequency
 
     def __iter__(self):
-
         data = (
             pd.date_range(self.start_date, self.end_date, freq=self.date_frequency)
             .strftime("%Y-%m-%d")  # type: ignore
             .tolist()
         )
 
         result = list(zip(itertools.repeat(self.date_param), data))
@@ -192,26 +189,25 @@
     ] = None  # (df column name, parameter name)
     start_date: Optional[str] = None
     end_date: Optional[str] = None
     date_param: Optional[str] = None
     date_frequency: Optional[str] = None
 
     def execute(self, previousQuery: Optional[BaseBqlQuery]) -> bool:
-
         generators = []
         if self.date_param is not None:
             assert self.start_date is not None and self.end_date is not None
             generators.append(DateGen(self.date_param, self.start_date, self.end_date))
         if self.copy_from_previous is not None:
-            if previousQuery is None or previousQuery.dataframe is None:
+            if previousQuery is None or previousQuery.to_df() is None:
                 raise ValueError(
                     "Unexpected, copy_from_previous defined, but previousQuery or previousQuery.dataframe is None"
                 )
 
-            parent_dataframe = previousQuery.dataframe
+            parent_dataframe = previousQuery.to_df()
             id_col = self.copy_from_previous[0]
             param_name = self.copy_from_previous[1]
 
             logger.info(UniqueColIter(id_col, param_name, parent_dataframe).__iter__())
 
             generators.append(UniqueColIter(id_col, param_name, parent_dataframe))
 
@@ -222,15 +218,15 @@
             queries = []
 
             logger.info("Generating queries")
             # Create the queries
             for resultparams in itertools.product(*generators):
                 # resultparams is a iterator of Tuples (from the generators)
                 logger.info(f"Running with parameters: {resultparams}")
-                for (param, value) in resultparams:
+                for param, value in resultparams:
                     if self.query.params is not None:
                         self.query.params[param] = value
 
                 # self.params[date_param] = date_value # pass the date to this query
                 query_copy = copy.deepcopy(self.query)
 
                 queries.append(query_copy)
@@ -244,25 +240,25 @@
             last_execution_status = BaseBqlQuery.STATUS_FAILURE
             for q in queries:
                 last_execution_status = q.execution_status
                 if last_execution_status != BaseBqlQuery.STATUS_COMPLETED:
                     logger.info(f"Query failed, stopping execution. {q.exception_msg}")
                     return False
 
-                qdf = q.dataframe
+                qdf = q.to_df()
                 for param_key, value in q.params.items():
                     if isinstance(value, list) and len(value) == 1:
                         value = value[0]
                     param = param_key.replace("$", "") + "_PARAM"
                     qdf[param] = value
 
                 dfs.append(qdf)
 
-            self.query.dataframe = pd.concat(dfs)
-            self.query.dataframe.reset_index(drop=True, inplace=True)
+            self.query._df = pd.concat(dfs)
+            self.query._df.reset_index(drop=True, inplace=True)
             self.query.execution_status = last_execution_status
 
         return True
 
 
 @dataclass
 class QueryPipeline:
@@ -296,21 +292,21 @@
             previousQuery = query.query
 
             if not success:
                 logger.warning(f"Failure executing previousQuery {previousQuery}")
                 return False
 
         # everything passed
-        assert previousQuery is not None and previousQuery.dataframe is not None
+        assert previousQuery is not None and previousQuery.to_df() is not None
         logger.debug("Pipeline execution passed successfully")
         return True
 
     def successful(self) -> bool:
         success = (
             self.queries[-1].query.execution_status == BaseBqlQuery.STATUS_COMPLETED
         )
         if not success:
             logger.warning(f"Failure: {self.queries[-1].query.exception_msg}")
         return success
 
     def dataframe(self) -> Optional[pd.DataFrame]:
-        return self.queries[-1].query.dataframe
+        return self.queries[-1].query.to_df()
```

## iql/bbg_bql/bql_extension.py

```diff
@@ -1,28 +1,26 @@
 # Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
 # All Rights Reserved
 
 import logging
 import re
-import os
-import csv
-
-import pandas as pd
 from pandas import DataFrame
-from typing import List, Union, Optional, Dict
+from typing import List, Optional, Dict
 from dataclasses import dataclass, field
 
 from iql import q_cache
-from iql.bbg_bql.bql_wrapper import (
-    BaseBqlQuery,
-    execute_bql_str_list_async_q,
-    list_to_str,
+from iql.bbg_bql.bql_wrapper import BaseBqlQuery, execute_bql_str_list_async_q
+from iql.bbg_bql.bql_datamodel import RawBqlQuery
+from iql.iqmoql import (
+    IqlExtension,
+    register_extension,
+    SubQuery,
+    get_subqueries_flat,
+    IqlQueryContainer,
 )
-from iql.bbg_bql.bql_datamodel import RawBqlQuery, QueryPipeline
-from iql.iqmoql import IqmoQlExtension, register_extension, SubQuery
 
 
 logger = logging.getLogger(__name__)
 
 _KEYWORD = "bql"
 
 _bql_start_pattern = r"(?si)\(\s*((get)|(let))\s*\("
@@ -37,177 +35,28 @@
 class _IqmoBqlQuery(SubQuery):
     # Extended BQL language to add "iqmo" options
     # such as "splitid" and pivoting
     # Syntax; pivot(id, name)
     # Syntax 2: pivot([id:col2], name)
     bqlquery: BaseBqlQuery = field(init=False)
 
-    def get_query(self) -> str:
-        """Overridden, so we can pull a list of ids from an external file"""
-        query_base = next(iter(self.options.keys()), None)
-        if query_base is None:
-            raise ValueError("No BQL query found")
-
-        if "paramfile" in self.options:
-            # id_fileparam is a tuple: a string to replace, and a filename to get the values from
-            paramname, filename = self.options.get("paramfile")  # type: ignore
-
-            if paramname not in query_base:
-                raise ValueError(
-                    f"Query doesn't contain the parameter name {paramname} clause, cannot substitute"
-                )
-
-            if type(filename) is not str:
-                raise ValueError(f"Unexpected type for fileparam: {type(filename)}")
-
-            if os.path.exists(filename):
-                logger.info(f"Using ids from {filename}")
-                with open(filename, "r") as file:
-                    reader = csv.reader(file)
-                    values = [v[0] for v in reader]
-
-                    id_list_str = list_to_str(values, quote=True)
-                    if paramname not in query_base:
-                        raise ValueError(
-                            "Query doesn't contain the parameter name {paramname} clause, cannot substitute"
-                        )
-                    else:
-                        newfor = f"[{id_list_str}]"
-                        logger.info(f"Replacement for list: {id_list_str}")
-
-                        return query_base.replace(paramname, newfor)
-
-            else:
-                raise ValueError(f"idlist does not exist {filename}")
-        else:
-            return query_base
-
-    def raw_dataframe(self) -> Union[DataFrame, None]:
-        return self.bqlquery.dataframe
-
-    def run_outside_batch(self) -> bool:
-        return False
-
-    def execute_paramlist(self) -> DataFrame:
-        # TODO: Allow this to be batched
-
-        logger.debug("Param list is enabled, splitting query into a two stage pipeline")
-
-        query = self.bqlquery.to_bql_query()
-
-        paramlist: List[str] = self.options.get("paramlist")  # type: ignore
-        paramquery: Optional[str] = self.options.get("paramquery")  # type: ignore
-        if paramlist is None and paramquery is not None:
-
-            if not isinstance(paramquery, list) and len(paramquery) != 2:
-                raise ValueError("paramquery must be a Tuple of (param, 'query')")
-
-            parameter_name = paramquery[0]
-            paramquery = paramquery[1]
-
-            df = self.extension.db_connection.sql(paramquery).to_df()  # type: ignore
-
-            parameter_list = df[df.columns[0]].values
-
-        elif paramlist is not None:
-
-            if not isinstance(paramlist, list) and len(paramlist) != 2:
-                raise ValueError("paramlist must be a Tuple of (param, [values])")
-
-            parameter_name = paramlist[0]
-            parameter_list = paramlist[1]
-
-        if parameter_name not in query:
-            raise ValueError(f"{parameter_name} not found in query, nothing to replace")
-
-        queries = []
-
-        for val in parameter_list:
-
-            new_query = query.replace(parameter_name, val)
-
-            logger.debug(f"Creating a raw query for {val}: {new_query}")
-
-            q = RawBqlQuery(new_query)
-            queries.append(q)
-
-        execute_bql_str_list_async_q(queries)
-
-        for q in queries:
-            if q.dataframe is None:
-                raise ValueError("BQL query failed, cannot continue")
-
-        dfs = [q.dataframe for q in queries]
-
-        df = pd.concat(dfs)
-
-        self.bqlquery.dataframe = df
-        return df
-
-    def execute_split(self) -> DataFrame:
-        # TODO: Allow this to be batched
-        logger.debug("Split is enabled, splitting query into a two stage pipeline")
-        pipeline = QueryPipeline()
-
-        # Extract For Clause
-        query = self.bqlquery.to_bql_query()
-
-        match = _QUERY_FOR_PATTERN.fullmatch(query)
-
-        if match is None:
-            raise ValueError(f"Could not extract FOR clause from {query}")
-        for_str = match.group(2)
-        with_str = match.group(3)
-        prefs_str = match.group(5)
-        rest_str = (
-            (with_str if with_str is not None else "")
-            + " "
-            + (prefs_str if prefs_str is not None else "")
-        )
-
-        q1_str = f"get (id) for ({for_str}) {rest_str}"
-        q1 = RawBqlQuery(q1_str)
-
-        pipeline.add_query(query=q1)
-
-        q2_str = query.replace(for_str, "['$SECURITY']")
-        q2 = RawBqlQuery(q2_str)
-        pipeline.add_query(query=q2, copy_from_previous=("id", "$SECURITY"))
-
-        pipeline.execute()
-
-        # df = pipeline.dataframe()
-        if pipeline.successful():
-            self.bqlquery.dataframe = pipeline.dataframe()
-            self.bqlquery.execution_status = self.bqlquery.STATUS_COMPLETED
-
-            if self.bqlquery.dataframe is None:
-                raise ValueError("Pipeline passed, but dataframe is still None")
-
-            return self.bqlquery.dataframe
-        else:
-
-            self.bqlquery.execution_status = self.bqlquery.STATUS_FAILURE
-            raise ValueError("Failure in execution")
-
     # detects everything before "(.*) as #..."
 
     def validate_fix_column_names(self, df) -> DataFrame:
         # BQL does two annoying things:
         # 1. It drops duplicate columns silently, even if the duplicates are desired or slightly different.
         # This detects this case, and throws an exception to force the query writer to handle it.
         # 2. It sometimes ignores the "alias", so this will re-insert the alias if needed
 
         if len(df) == 0:
             return df
 
         cols_returned = list(df["name"].unique())
         cols_expected = self.bqlquery.get_fields()
         if len(cols_returned) != len(cols_expected):
-
             raise ValueError(
                 f"""Unexpected number of columns returned. Expected {len(cols_expected)}, 
                 got {len(cols_returned)}. Got: {df['name'].unique()}, expected {cols_expected}"""
             )
 
         if (
             True
@@ -232,15 +81,15 @@
         # populate_from_cache is called from execute_batch, doesn't need to be run again here
         if self.dataframe is not None:
             return True
 
         success = self.execute_internal()
 
         if success:
-            df = self.bqlquery.dataframe
+            df = self.bqlquery.to_df()
 
             df = self.extension.apply_pandas_operations_prepivot(df, self.options)
 
             df = self.extension.pivot(df, self.options.get("pivot"))  # type: ignore
             df = self.extension.apply_pandas_operations_postpivot(df, self.options)
 
             self.dataframe = df
@@ -250,15 +99,14 @@
         else:
             allow_failure_opt = self.options.get("allow_failure")
             if allow_failure_opt is None or (
                 isinstance(allow_failure_opt, bool) and allow_failure_opt is False
             ):
                 return False
             else:
-
                 if isinstance(allow_failure_opt, bool) and allow_failure_opt is True:
                     logger.info(
                         "Query failed, but allow_failure is enabled. Creating an empty dataframe with one id column."
                     )
                     self.dataframe = DataFrame(columns=["id"])
                 else:
                     if isinstance(allow_failure_opt, str):
@@ -269,109 +117,108 @@
                         f"Query failed, but allow_failure is enabled. Creating an empty dataframe with cols = {cols}"
                     )
 
                     self.dataframe = DataFrame(columns=cols)
                 return True
 
     def execute_internal(self) -> bool:
-
         if self.bqlquery.execution_status == BaseBqlQuery.STATUS_FAILURE:
             return False
 
         if self.bqlquery.execution_status == BaseBqlQuery.STATUS_COMPLETED:
             return True
 
-        if not self.run_outside_batch():
-            logger.debug(
-                "Query is not executed/cached, this should only occur when a single BQL query is executed"
-            )
-
         working_df = None
 
         # If it already ran, don't run again
         if not self.bqlquery.execution_status == BaseBqlQuery.STATUS_COMPLETED:
             # logger.info("Not splitting")
             success = self.bqlquery.execute()
 
             if not success:
                 logger.debug(f"Result {success}")
                 return False
 
         # query has passed
         if working_df is None:
-            working_df = self.bqlquery.dataframe
+            working_df = self.bqlquery.to_df()
 
         assert working_df is not None
 
         # validate column names: disabled for now, still a work in progress
         # working_df = self.validate_fix_column_names(working_df)
-
         self.dataframe = working_df
-
         return True
 
 
 @dataclass
-class BqlExtension(IqmoQlExtension):
-    def create_subqueries(
-        self, query: str, name: str, con: object
-    ) -> List[_IqmoBqlQuery]:
-
-        # Use the super() implementation, to reuse the paramlist splitting.
-        sqs = super().create_subqueries(query, name, con)
-
-        iqs = []
-        for sq in sqs:
-            iq = _IqmoBqlQuery(
-                subquery=sq.subquery, name=sq.name, extension=self, dbcon=con
-            )
-
-            bqlstr = iq.get_query()
-            q = RawBqlQuery(bqlstr)
-            iq.bqlquery = q
+class BqlExtension(IqlExtension):
+    def create_subquery(
+        self, subquery: str, name: str, iqc: IqlQueryContainer
+    ) -> SubQuery:
+        iq = _IqmoBqlQuery(subquery=subquery, name=name, extension=self, iqc=iqc)
+
+        bqlstr = iq.get_query()
+        q = RawBqlQuery(bqlstr)
+        iq.bqlquery = q
+        return iq
 
-            iqs.append(iq)
-        return iqs
+    def create_subqueries(
+        self,
+        query: str,
+        name: str,
+        iqc: IqlQueryContainer,
+        create_function: object = None,
+    ) -> List["SubQuery"]:
+        return super().create_subqueries(
+            query=query, name=name, iqc=iqc, create_function=self.create_subquery
+        )
 
     def execute_batch(self, subqueries: List[_IqmoBqlQuery]) -> Dict[str, DataFrame]:
         # Caching operates at two levels here:
         # The SubQuery result, and within the bql_wrapper
         # To force a refresh, we'll clear both the subquery and bql raw query
         # cache
-        for sq in subqueries:
+
+        subqueries_flat: List[_IqmoBqlQuery] = get_subqueries_flat(subqueries)  # type: ignore
+
+        for sq in subqueries_flat:
             sq.populate_from_cache()
 
-        needs_to_be_cleared = [
-            q for q in subqueries if not self.allow_cache_read_inner(q)
-        ]
+        clear_inner_caches = False
+
+        needs_to_be_cleared = [q for q in subqueries_flat if clear_inner_caches]
         logger.debug(f"Clearing {len(needs_to_be_cleared)}")
         # clear lower-level cache entries
         for q in needs_to_be_cleared:
             q_cache.clear(q.bqlquery.to_bql_query())
 
         to_run: List[_IqmoBqlQuery] = [
-            sq
-            for sq in subqueries
-            if sq.dataframe is None and not sq.run_outside_batch()
+            sq for sq in subqueries_flat if sq.dataframe is None
         ]
 
         queries = [q.bqlquery for q in to_run]
 
         # We already checked whether its cached AND whether caching is allowed in sq.populate_from_cache
         logger.debug(f"Executing {len(queries)}")
         execute_bql_str_list_async_q(queries)
 
-        completed_dfs = {}
         # Then update the subqueries
-        for q in subqueries:
+        for q in subqueries_flat:
             if q.bqlquery.execution_status == BaseBqlQuery.STATUS_FAILURE:
-                raise ValueError(
-                    f"BQL SubQuery failed {q.bqlquery.exception_msg}: {q.bqlquery.to_bql_query()}"
-                )
+                if q.options.get("allow_failure") is None:
+                    raise ValueError(
+                        f"BQL SubQuery failed {q.bqlquery.exception_msg}: {q.bqlquery.to_bql_query()} {q.options}"
+                    )
             q.execute()
+
+        completed_dfs = {}
+        # Final step to merge any grouped subqueries.
+        for q in subqueries:
+            q.merge()
             df = q.dataframe
             completed_dfs[q.name] = df
 
         return completed_dfs
 
 
 def execute_bql(query: str, pivot: Optional[str] = None) -> DataFrame:
@@ -386,18 +233,18 @@
     else:
         suffix = ""
 
     query = f'{_KEYWORD}("{query}"{suffix})'
     extension = BqlExtension(_KEYWORD)
 
     logger.debug(f"Converted to: {query}")
-    sqs = extension.create_subqueries(query, "Anon", con=None)
+    sqs = extension.create_subqueries(query, "Anon", iqc=None)  # type: ignore
     sq = sqs[0]
 
-    sq.execute()
+    sq.execute()  # type: ignore
 
     if sq.dataframe is None:
         raise ValueError(f"Unable to execute {sq.subquery}")
 
     return sq.dataframe
 
 
@@ -405,15 +252,15 @@
     """Batch executes multiple BQL Queries. Much faster than running serially."""
     extension = BqlExtension(_KEYWORD)
 
     wrapped_queries = [f'{_KEYWORD}("{q}")' for q in queries]
 
     iqs = []
     for query in wrapped_queries:
-        sqs = extension.create_subqueries(query, "Anon", con=None)
+        sqs = extension.create_subqueries(query, "Anon", iqc=None)  # type: ignore
         iqs.extend(sqs)
 
     extension.execute_batch(iqs)
 
     return {sq.subquery: sq.dataframe for sq in iqs}
```

## iql/bbg_bql/bql_wrapper.py

```diff
@@ -2,75 +2,86 @@
 # All Rights Reserved
 
 """ This module wraps the Bloomberg BQL API to provide
 consistent return results """
 
 import time
 import logging
-
+from threading import Lock
 from datetime import datetime
 from functools import partial
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Dict
 from pandas import DataFrame
-
 from abc import abstractmethod
 
 import bql  # pyright: ignore pylint: disable=C0413 # noqa: E402
 from iql import q_cache
+from iql import iqmoql
 
-# from bbg_bql.datamodel import RawBqlQuery, BaseBqlQuery, BqlQuery, _PipelineBqlQuery
 
 _MAX_CONCURRENT = 128
 _SHIFT_DUPLICATES = True
-_CACHE_PERIOD = None
 
 logger = logging.getLogger(__name__)
 
 bqService = None
+_disabled = False
+
+# Used to avoid multiple threads from simultaneously running bql statements
+bqllock = Lock()
 
 
 class BaseBqlQuery:
     STATUS_NOTRUN = "NOTRUN"
     STATUS_COMPLETED = "COMPLETED"
     STATUS_FAILURE = "FAILURE"
 
     execution_status: str = STATUS_NOTRUN
     exception_msg: Optional[str] = None
-    dataframe: Optional[DataFrame] = None
+    _data: Optional[List[Dict[str, object]]] = None
+    _df: Optional[DataFrame] = None
 
     params = None
 
     @abstractmethod
     def get_fields(self) -> List[str]:
         pass
 
     @abstractmethod
     def to_bql_query(self) -> str:
         pass
 
     def execute(self) -> bool:
-        """Executes the query and, if successful, sets the query.dataframe"""
+        """Executes the query and, if successful, sets the query._data"""
         try:
-            self._populate_df()
-            # logger.info(f"Done executing {self.dataframe}")
+            self._populate_data()
             return self.execution_status == self.STATUS_COMPLETED
         except Exception as e:
-            logger.exception("to_dataframe")
+            logger.exception("execute")
             self.execution_status = self.STATUS_FAILURE
             self.exception_msg = str(e)
             return False
 
-    def to_df(self) -> DataFrame:
-        success = self.execute()
-        if not success or self.dataframe is None:
-            raise ValueError("Failure executing BQL query")
+    def to_data(self) -> List[Dict[str, object]]:
+        """Internal representation"""
+        if self._data is not None:
+            return self._data
         else:
-            return self.dataframe
+            success = self.execute()
+            if not success or self._data is None:
+                raise ValueError("Failure executing BQL query")
+            else:
+                return self._data
 
-    def _populate_df(self):
+    def to_df(self) -> DataFrame:
+        if self._df is None:
+            self._df = DataFrame(self._data)
+        return self._df
+
+    def _populate_data(self):
         execute_bql_str_list_async_q([self])
 
 
 def get_bqservice(retries: int = 3):
     global bqService
     logger.debug("Creating new bqService")
 
@@ -97,15 +108,15 @@
     try:
         global bqService
         if bqService is None or bqService._Service__bqapi_session is None:  # type: ignore
             logger.info("_Service__bqapi_session already closed or None")
             return
         else:
             logger.info("Closing _Service__bqapi_session session")
-            bqService._Service__bqapi_session.close()   # type: ignore
+            bqService._Service__bqapi_session.close()  # type: ignore
             bqService = None
     except Exception:
         logger.exception("Error closing bqapi session")
 
 
 def list_to_str(values: list, quote: bool = False, delimiter: str = ", \n") -> str:
     """Helper to convert list of values to a comma delimited list. Used for BQL functions.
@@ -191,30 +202,36 @@
 
 
 def execute_bql_str_list_async_q(
     queries_input: List[BaseBqlQuery],
     suppress_warning_log: bool = False,
     max_queries: int = _MAX_CONCURRENT,
 ):
-    """Note: Not multi-process safe due to underlying BQL APIs 
-    and (presumably) its use a Singleton for bqapi requests. 
+    if _disabled:
+        raise ValueError("BQL is disabled")
+    """Note: Not multi-process safe due to underlying BQL APIs
+    and (presumably) its use a Singleton for bqapi requests.
     Either batch requests through a single requester thread, or
     distribute workload across requesters.
     """
     logger.debug("Checking to see if any are already cached")
 
     for q in queries_input:
         qstr = q.to_bql_query()
-        df: Optional[DataFrame] = q_cache.get(qstr)  # type: ignore
-        if df is not None:
+        data = q_cache.get(qstr)  # type: ignore
+        if data is not None:
             logger.debug(f"Found in cache: {qstr}")
-            q.dataframe = df
+
+            if isinstance(data, DataFrame):
+                q._df = data
+            else:
+                q._data = data  # type: ignore
             q.execution_status = q.STATUS_COMPLETED
 
-    queries_not_cached = [q for q in queries_input if q.dataframe is None]
+    queries_not_cached = [q for q in queries_input if q._data is None]
 
     """Max Queries indicates the max per batch: chop the queries
     into smaller groups of max_queries size and execute each serially"""
 
     if len(queries_not_cached) == 0:
         logger.debug("No queries to run")
         return
@@ -241,20 +258,20 @@
         _execute_bql_str_list_async_orig(query_group, suppress_warning_log)
 
     end = time.time()
     logger.info(f"Elapsed time running queries: {end-start} seconds")
 
     for q in queries_not_cached:
         logger.debug("Saving to cache")
-        if q.dataframe is not None:
+        if q._data is not None:
             q_cache.save(
                 q.to_bql_query(),
-                q.dataframe,
+                q._data,
                 type=__name__,
-                duration_seconds=_CACHE_PERIOD,
+                duration_seconds=iqmoql._CACHE_PERIOD,
             )
 
     return
 
 
 def submit_fetch_many_available():
     # Force execute_many for now.
@@ -262,59 +279,60 @@
 
     return False
 
 
 def _execute_bql_str_list_async_orig(
     queries: List[BaseBqlQuery], suppress_warning_log: bool = False
 ):
-    query_strings = []
-    for query in queries:
-        qstr = query.to_bql_query()
-
-        if "iqmo" in qstr:
-            raise ValueError("IQMO parameters passed to BQL layer, cannot run")
-
-        logger.debug(f"Executing {qstr}")
-        query_strings.append(qstr)
-
-    bqService = get_bqservice()
-    # error_list: List[str] = []
-
-    if submit_fetch_many_available():
-        logger.debug("Using submit fetch many")
-        gen = bqService.submit_fetch_many(
-            query_strings, on_request_error=error_callback
-        )
-    else:
-        gen = bqService.execute_many(
-            query_strings,
-            partial(error_callback),
-        )
+    with bqllock:
+        query_strings = []
+        for query in queries:
+            qstr = query.to_bql_query()
+
+            if "iqmo" in qstr:
+                raise ValueError("IQMO parameters passed to BQL layer, cannot run")
+
+            logger.debug(f"Executing {qstr}")
+            query_strings.append(qstr)
+
+        bqService = get_bqservice()
+        # error_list: List[str] = []
+
+        if submit_fetch_many_available():
+            logger.debug("Using submit fetch many")
+            gen = bqService.submit_fetch_many(
+                query_strings, on_request_error=error_callback
+            )
+        else:
+            gen = bqService.execute_many(
+                query_strings,
+                partial(error_callback),
+            )
 
-    error_index = 0
+        error_index = 0
 
-    logger.info("Processing results")
-    for r, q in zip(gen, queries):
-        try:
-            if r is None:
+        logger.info("Waiting for and processing BQL results")
+        for r, q in zip(gen, queries):
+            try:
+                if r is None:
+                    q.execution_status = q.STATUS_FAILURE
+                    logger.warn(f"Error executing: {q.to_bql_query()}")
+                    q.exception_msg = "Failure"
+                    error_index = error_index + 1
+                else:
+                    data = _to_data(r)
+                    q._data = data
+                    q.execution_status = q.STATUS_COMPLETED
+
+            except Exception as e:
+                logger.exception("Query error")
+                q._data = None
                 q.execution_status = q.STATUS_FAILURE
-                logger.warn(f"Error executing: {q.to_bql_query()}")
-                q.exception_msg = "Failure"
-                error_index = error_index + 1
-            else:
-                df = _to_dataframe(r)
-                q.dataframe = df
-                q.execution_status = q.STATUS_COMPLETED
-
-        except Exception as e:
-            logger.exception("Query error")
-            q.dataframe = None
-            q.execution_status = q.STATUS_FAILURE
-            q.exception_msg = str(e)
-    logger.info("Done executing")
+                q.exception_msg = str(e)
+        logger.info("Done executing")
 
 
 def flatten_list_str(value: Union[str, List[str]]) -> List[str]:
     """Converts input to a List, if not already a List"""
     if isinstance(value, str):
         value_str = str(value)
 
@@ -407,15 +425,14 @@
         if isinstance(res, bql.SingleItemResponse):
             _process_single_item_response(res, result_table)
         else:
             # Sometimes, there are multiple levels to the responses
             _process_response(res, result_table)
 
 
-def _to_dataframe(response: bql.Response) -> DataFrame:
+def _to_data(response: bql.Response) -> List[Dict[str, object]]:
     """Converts BQL Response to a List of Dicts, where each dict contains Col: Value"""
     result_table: List = []
 
     _process_response(response, result_table)
 
-    df = DataFrame(result_table)
-    return df
+    return result_table
```

## iql/db_connectors/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-# Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
-# All Rights Reserved
+# Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
+# All Rights Reserved
```

## iql/db_connectors/duckdb_connector.py

```diff
@@ -1,53 +1,91 @@
 # Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
 # All Rights Reserved
 
 import duckdb
 import logging
-from typing import Dict, List
+from contextlib import nullcontext
+from typing import Dict, Optional
+
 from pandas import DataFrame
-from iql.iqmoql import DatabaseConnector
+
+from iql.iqmoql import IqlDatabaseConnector, IqlDatabase, IqlResult
+import threading
+
+from dataclasses import dataclass
 
 logger = logging.getLogger(__name__)
 
 
-class _DuckDbConnector(DatabaseConnector):
-    def get_connection(self) -> object:
-        """Used for executing multiple queries against the same database"""
-        con = duckdb.connect(database=":memory:")
-        return con
+@dataclass
+class _DuckDB(IqlDatabase):
+    _connection: object
+    _started_thread: int
 
-    def close_connection(self, con):
+    def execute_query(
+        self, query: str, completed_dfs: Optional[Dict[str, DataFrame]] = None
+    ) -> Optional[IqlResult]:
+        """param: Each of the completed _dfs are registered to the database.
+        threaded: pass True to run in a separate connection, otherwise runs in main connection
+        """
+
+        threaded = threading.get_ident() != self._started_thread
+
+        # create & close the connection if we're threading, otherwise create one
+        with self.get_connection() if threaded else nullcontext(
+            self._connection
+        ) as con:
+            try:
+                # Register each of the dataframes to duckdb, so duckdb can query them
+                # Other database might require a "load" or "from_pandas()" step to load these
+                # to temporary tables.
+                if completed_dfs is not None:
+                    for key, df in completed_dfs.items():
+                        if df is None or (df.empty and len(df.columns) == 0):
+                            continue
+                            # raise ValueError(f"None dataframe for {key}")
+                        con.register(key, df)  # type: ignore
+
+                d = con.execute(query)  # type: ignore
+                # Don't use con.sql, as it adds a small but
+                # measurable overhead of creating a duckdb relation, that we don't need
+                if d is not None:
+                    # logger.debug("Using Pandas format")
+                    try:
+                        table = d.arrow()
+                        return IqlResult(_table=table)
+                    except Exception:
+                        # TODO: Detect this more gracefully
+                        logger.debug("Didn't have a result set {str(e)}")
+                        return None
+
+                else:
+                    return None
+            except Exception as e:
+                logger.exception(f"Error executing SQL DFs: {query}")
+                raise e
+
+    def get_connection(self):
+        return self._connection.cursor()  # type: ignore
+
+    def close_db(self):
         try:
-            if con is None:
+            if self._connection is None:
                 return
-
-            con.close()
+            else:
+                self._connection.close()  # type: ignore
+                self._connection = None
         except Exception:
             logger.exception("Unable to close")
 
-    def execute_query(
-        self, con: object, query: str, completed_dfs: Dict[str, DataFrame]
-    ) -> List[DataFrame]:
-        try:
-            # Register each of the dataframes to duckdb, so duckdb can query them
-            # Other database might require a "load" or "from_pandas()" step to load these
-            # to temporary tables.
-            for key, df in completed_dfs.items():
-                if df is None:
-                    continue
-                    # raise ValueError(f"None dataframe for {key}")
-                con.register(key, df)  # type: ignore
-
-            r = con.query(query)  # type: ignore
-            if r is not None:
-                df = r.to_df()
-                return [df, *completed_dfs.values()]
-            else:
-                return []
-        except Exception as e:
-            logger.exception(f"Error executing SQL DFs: {query}")
-            raise e
+
+class _DuckDbConnector(IqlDatabaseConnector):
+    def create_database(self) -> _DuckDB:
+        con = duckdb.connect(database=":memory:")
+        return _DuckDB(_connection=con, _started_thread=threading.get_ident())
+
+    def create_database_from_con(self, con: object) -> _DuckDB:
+        return _DuckDB(_connection=con, _started_thread=threading.get_ident())
 
 
-def getConnector() -> DatabaseConnector:
+def getConnector() -> IqlDatabaseConnector:
     return _DuckDbConnector()
```

## iql/extensions/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-# Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
-# All Rights Reserved
+# Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
+# All Rights Reserved
```

## iql/extensions/aws_s3_extension.py

```diff
@@ -1,45 +1,53 @@
 # Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
 # All Rights Reserved
 
 import logging
 from dataclasses import dataclass
 from pandas import DataFrame
 from typing import Tuple, Optional, Dict
-from iql.iqmoql import IqmoQlExtension, register_extension, SubQuery
+from iql.iqmoql import IqlExtension, register_extension, SubQuery
 import boto3
 import re
 import os
 from pathlib import Path
 from iql import q_cache
 
 logger = logging.getLogger(__name__)
 
 _PATTERN = re.compile(r"s3://(.*?)/(.*)")
 
 BOTO3_S3_RESOURCES: Dict[str, object] = {}
 BOTO3_S3_RESOURCE_DEFAULT = None
 
+
 def get_boto3_resource_for_request(url: str) -> object:
     """boto3 resources may be pre-created and saved in
     aws_s3_extension.BOTO3_S3_RESOURCES.
     Or, override this for your custom implementation."""
     for prefix, boto3obj in BOTO3_S3_RESOURCES:
         if url.startswith(prefix):
+            logger.debug("Using overridden")
             return boto3obj
-    else:
-        # Return the default
-        return boto3.resource("s3")
+        elif BOTO3_S3_RESOURCE_DEFAULT is not None:
+            logger.debug("Using BOTO3_S3_RESOURCE_DEFAULT")
+            return BOTO3_S3_RESOURCE_DEFAULT
+
+    logger.debug("Using default")
+    return boto3.resource("s3")
 
 
 @dataclass
-class AwsS3Extension(IqmoQlExtension):
-    def get_path_replacement(self, subquery: str) -> str:
-        bucket, key, local_path = self.options_to_tuple(subquery)
-        return local_path
+class AwsS3Extension(IqlExtension):
+    def get_path_replacement(self, subquery: SubQuery, quote: bool = True) -> str:
+        bucket, key, local_path = self.options_to_tuple(subquery.get_query())
+        if quote:
+            return f"'{local_path}'"
+        else:
+            return local_path
 
     def use_path_replacement(self) -> bool:
         return True
 
     def options_to_tuple(self, subquery: str) -> Tuple[str, str, str]:
         # returns bucket, key, local filename
 
@@ -60,32 +68,31 @@
             local_path = filename
         else:
             local_path = os.path.join(self.temp_file_directory, filename)
 
         return (bucket, key, local_path)
 
     def execute(self, sq: SubQuery) -> Optional[DataFrame]:
-
         url = sq.get_query()
         bucket, key, local_path = self.options_to_tuple(url)
 
         # For path replacement cases, the q_cache just stores a reference to the path.
         # when the file is expired, q_cache returns None
         obj = q_cache.get(local_path)
         expired = obj is None  # if obj is None, then the file is expired
 
         if Path(local_path).exists() and not expired and self.allow_cache_read(sq):
             logger.info(f"{local_path} exists, not downloading again")
             return None
         else:
-            logger.info(f"Downloading {key} to {local_path}")
+            logger.debug(f"Downloading {key} to {local_path} from bucket {bucket}")
 
             s3_resource = get_boto3_resource_for_request(url)
-
-            s3_resource.Bucket(bucket).download_file(key, local_path)  # type: ignore
+            s3_bucket = s3_resource.Bucket(bucket)  # type: ignore
+            s3_bucket.download_file(key, local_path)  # type: ignore
 
             # Just save the path name as the object
             q_cache.save(
                 local_path,
                 local_path,
                 self.get_cache_period(),
                 self.use_file_cache(),
```

## iql/extensions/edgar_extension.py

```diff
@@ -4,15 +4,15 @@
 import requests
 import logging
 import numpy
 import re
 import os
 from typing import Dict, List, Optional
 from pandas import DataFrame  # read_fwf
-from iql.iqmoql import IqmoQlExtension, register_extension, SubQuery
+from iql.iqmoql import IqlExtension, register_extension, SubQuery
 from iql.extensions import fred_extension as fe
 
 # import base64
 # from io import BytesIO
 # import pathlib
 
 logger = logging.getLogger(__name__)
@@ -56,56 +56,55 @@
     When it encounters a list, it creates a Dict for each list element combined with the stacks key/values.
     If the list contains anything other than a Dict, raises an Exception"""
 
     if type(d) is dict:
         vals = {}
         for k, v in d.items():
             # First, capture the scalar values at this level and push onto the stack
-            if not type(v) is dict and not type(v) is list:
+            if type(v) is not dict and type(v) is not list:
                 # Scalar
                 vals[k] = v
         stack.append(vals)
 
         # Next, process any dict items:
 
         for k, v in d.items():
             # Store the dict key as the name for the level
             if type(v) is dict:
                 vals[f"level_{len(stack)}"] = k
                 flatten_to_first_list(v, stack, rows)
             if type(v) is list:
-
                 # Assumes each element in the list is a dict
                 for i in v:
                     rowvals = {}
                     for s in stack:
                         rowvals.update(s)
 
                     rowvals["list"] = k
                     if numpy.isscalar(i):
                         rowvals["val"] = i
-                    elif not type(i) is dict:
+                    elif type(i) is not dict:
                         raise ValueError(f"Unexpected list element type: {type(i)}")
                     else:
                         rowvals.update(i)
 
                     rows.append(rowvals)
     stack.pop()
 
 
 def to_df(json) -> DataFrame:
     """Converts an Edgar JSON response to a DataFrame"""
     stack = []
     rows = []
+
     flatten_to_first_list(json, stack, rows)
     return DataFrame(rows)
 
 
 def _request_edgar(url: str) -> object:
-
     if EDGAR_USER_AGENT is None:
         raise ValueError(
             """Set iql.extension.edgar_extension.user_agent to: 'Your Company 'your@email.address') . 
             See https://www.sec.gov/os/webmaster-faq#developers for more info."""
         )
 
     global prefix
@@ -120,34 +119,33 @@
         raise ValueError(f"Error: {response.status_code}: {response.content.decode()}")
     else:
         # display(response.encoding)
         return response
 
 
 def edgar_request_to_df(url: str) -> DataFrame:
-
     rawdata = _request_edgar(url)
     data = rawdata.json()  # type: ignore
 
     if "filings" in data:
         if "recent" in data["filings"]:
-            return DataFrame.from_dict(
-                data["filings"]["recent"], orient="index"
-            ).transpose()
+            d = data["filings"]["recent"]
+
+            return DataFrame.from_dict(d, orient="index").transpose()
 
     df = to_df(data)
     return df
 
 
 # lastresponse = None
 
 lookup_re = re.compile(r"\s*(.*)\:(.*?)\:\s*")
 
 
-class EdgarExtension(IqmoQlExtension):
+class EdgarExtension(IqlExtension):
     """Keyword: the function name used in the SQL, such as query_somesite(...)
     base_url: The constant part of the URL path, such as https://www.somesite.com/abc/api
     path: The variable part of the URL path, which will be passed in the function as: query_somesite(path='/data/something',
 
     """
 
     keyword: str
@@ -157,22 +155,20 @@
     constant_params: Dict[str, str]
 
     # Params that will always be passed, such as:
     # api_key: somekey
     # or file_type: json
 
     def executeimpl(self, sq: SubQuery) -> DataFrame:
-
         constants_to_add = {}
 
         url = fe.get_url(sq, constants_to_add, _EDGAR_TYPES)
 
         # for https://www.sec.gov/Archives/edgar/cik-lookup-data.txt"
         if url.endswith(".txt"):
-
             res = _request_edgar(url)
             # data_str = StringIO(res.text)
 
             tempfilename = url[url.rindex("/") + 1 :]
 
             if self.temp_file_directory is None:
                 tempfilepath = tempfilename
```

## iql/extensions/fred_extension.py

```diff
@@ -2,18 +2,17 @@
 # All Rights Reserved
 
 import requests
 import logging
 from dataclasses import dataclass
 from typing import List, Dict
 from pandas import DataFrame
-from iql.iqmoql import IqmoQlExtension, register_extension, SubQuery
+from iql.iqmoql import IqlExtension, register_extension, SubQuery
 
 logger = logging.getLogger(__name__)
-
 FRED_API_KEY = None
 
 _FRED_TYPES = [
     {
         "name": "releases",
         "reqoptions": {},
         "url": "https://api.stlouisfed.org/fred/releases",
@@ -30,15 +29,14 @@
     },
 ]
 
 
 def options_to_url(
     type_name: str, sq: SubQuery, options_def: List[Dict], constants_to_add: Dict
 ) -> str:
-
     name, reqoptions, url = next(
         (
             (v["name"], v["reqoptions"], v["url"])
             for v in options_def
             if v["name"] == type_name
         ),
         (None, None, None),
@@ -56,15 +54,14 @@
             query_string = query_string.replace(ro_v, sq.options.get(ro_k))  # type: ignore
             constants_to_add[ro_k] = sq.options.get(ro_k)  # type: ignore
 
     return query_string
 
 
 def get_url(sq: SubQuery, constants_to_add: Dict, types: List[Dict]) -> str:
-
     first_option_k, first_option_v = next(
         ((k, v) for k, v in sq.options.items()), (None, None)
     )
     if first_option_v is None:
         fred_url = first_option_k  # type: ignore
     else:
         fred_url = sq.options.get("url")  # type: ignore
@@ -85,15 +82,15 @@
     else:
         query_string: str = fred_url  # type: ignore
 
     return query_string
 
 
 @dataclass
-class FredExtension(IqmoQlExtension):
+class FredExtension(IqlExtension):
     keyword: str
 
     def executeimpl(self, sq: SubQuery) -> DataFrame:
         constants_to_add = {}
 
         query_string = get_url(sq, constants_to_add, _FRED_TYPES)
         if FRED_API_KEY is None:
```

## iql/extensions/kaggle_extension.py

```diff
@@ -4,15 +4,15 @@
 import os
 import logging
 import pandas as pd
 
 from typing import List
 from dataclasses import dataclass
 from pandas import DataFrame
-from iql.iqmoql import IqmoQlExtension, register_extension, SubQuery
+from iql.iqmoql import IqlExtension, register_extension, SubQuery
 
 logger = logging.getLogger(__name__)
 
 _KAGGLE_API = None
 
 
 def set_kaggle_credentials(kaggle_username: str, kaggle_key: str):
@@ -21,29 +21,30 @@
 
 
 def get_api() -> "kaggle.api_client.ApiClient":  # type: ignore  # noqa: F821
     """Defer importing until after credentials are set, otherwise
     Kaggle's __init__ will raise an authentication exception."""
     global _KAGGLE_API
     if _KAGGLE_API is None:
-        import kaggle
+        import kaggle  # type: ignore
 
         api = kaggle.api
         _KAGGLE_API = api
 
     return _KAGGLE_API
 
 
 @dataclass
-class KaggleExtension(IqmoQlExtension):
+class KaggleExtension(IqlExtension):
     keyword: str
 
     def executeimpl(self, sq: SubQuery) -> DataFrame:
         """Retrieves and loads the DataSet File to a Pandas DataFrame.
-        Could be modified to retrieve a file path, similar to the AWS S3 Extension, for large files that cannot fit into memory."""
+        Could be modified to retrieve a file path, similar to the AWS S3 Extension, for large files that cannot fit into memory.
+        """
         api = get_api()  # type :ignore
         global _KAGGLE_API
 
         url = sq.get_query()
 
         query_array = url.split("/")
```

## iql/extensions/pandas_extension.py

```diff
@@ -1,44 +1,81 @@
 # Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
 # All Rights Reserved
 
 import logging
 from dataclasses import dataclass
 from pandas import DataFrame
-from iql.iqmoql import IqmoQlExtension, register_extension, SubQuery
+from iql.iqmoql import IqlExtension, register_extension, SubQuery, IqlDatabase
+import pyarrow as pa
+import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 
+def get_data(sq: SubQuery, source_query) -> pd.DataFrame:
+    db: IqlDatabase = sq.iqc.db  # type: ignore
+    input_data = sq.input_data
+    local_dfs = sq.local_dfs
+
+    # So much work to get Polars and/or PyArrow to work in sklearn
+    # Can revisit, but need to work around using onehotencoder
+    if input_data is not None:
+        if isinstance(input_data, DataFrame):
+            return input_data
+        elif isinstance(input_data, pa.lib.Table):
+            return input_data.to_pandas()  # type: ignore
+        else:
+            raise ValueError(f"Unexpected type: {type(input_data)}")
+
+    else:
+        result = db.execute_query(  # type: ignore
+            query=source_query, completed_dfs=local_dfs
+        )
+        if result is None:
+            raise ValueError(f"Could not get data for query {source_query}")
+        else:
+            return result.df_numpy()
+
+
+def get_query_from_options(options) -> str:
+    sql = options.get("sql")
+    if sql is not None:
+        return sql
+
+    dfname = options.get("df")
+    tablename = options.get("table")
+
+    if dfname is not None:
+        return f"select * from {dfname}"
+    elif tablename is not None:
+        return f"select * from {tablename}"
+
+    dataname = options.get("data")
+    if dataname is not None:
+        if " " in dataname:
+            return dataname
+        else:
+            return f"select * from {dataname}"
+
+    raise ValueError("df, table, sql and data are not specified")
+
+
 @dataclass
-class PandasExtension(IqmoQlExtension):
+class PandasExtension(IqlExtension):
     keyword: str
 
     def allow_cache_read(self, sq: SubQuery) -> bool:
         # Never cache, because this depends on contents of table
         return False
 
     def allow_cache_save(self, sq: SubQuery) -> bool:
         return False
 
     def executeimpl(self, sq: SubQuery) -> DataFrame:
-        dfname = sq.options.get("df")
-        tablename = sq.options.get("table")
-        sql = sq.options.get("sql")
-
-        if dfname is not None:
-            query = f"select * from {dfname}"
-        elif tablename is not None:
-            query = f"select * from {tablename}"
-        elif sql is not None:
-            query = sql
-        else:
-            raise ValueError("Must specify one of: df=, table= or sql=")
+        query = get_query_from_options(sq.options)
 
-        # TODO: This is hardcoded for DuckDB. Should rewrite to use iqmoql.DbConnector
-        df = sq.dbcon.sql(query).to_df()  # type: ignore
-        return df
+        return get_data(sq, query)
 
 
 def register(keyword: str):
     extension = PandasExtension(keyword=keyword)
     register_extension(extension)
```

## iql/extensions/template_extension.py

```diff
@@ -1,31 +1,29 @@
-# Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
-# All Rights Reserved
-
-import requests
-import logging
-from dataclasses import dataclass
-from typing import List, Dict
-from pandas import DataFrame
-from iql.iqmoql import IqmoQlExtension, register_extension, SubQuery
-
-logger = logging.getLogger(__name__)
-
-@dataclass
-class TemplateExtension(IqmoQlExtension):
-    keyword: str
-
-    def executeimpl(self, sq: SubQuery) -> DataFrame:
-        
-        # Get any options from sq
-        # model = sq.options.get("type")
-
-        # Do stuff
-        
-        # Return a DataFrame
-        
-        raise ValueError("Implement me")
-
-
-def register(keyword: str):
-    extension = TemplateExtension(keyword=keyword)
-    register_extension(extension)
+# Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
+# All Rights Reserved
+
+import logging
+from dataclasses import dataclass
+from pandas import DataFrame
+from iql.iqmoql import IqlExtension, register_extension, SubQuery
+
+logger = logging.getLogger(__name__)
+
+
+@dataclass
+class TemplateExtension(IqlExtension):
+    keyword: str
+
+    def executeimpl(self, sq: SubQuery) -> DataFrame:
+        # Get any options from sq
+        # model = sq.options.get("type")
+
+        # Do stuff
+
+        # Return a DataFrame
+
+        raise ValueError("Implement me")
+
+
+def register(keyword: str):
+    extension = TemplateExtension(keyword=keyword)
+    register_extension(extension)
```

## Comparing `iql-0.1.6.dist-info/LICENSE` & `iql-0.1.9b5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `iql-0.1.6.dist-info/METADATA` & `iql-0.1.9b5.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,656 +1,769 @@
-Metadata-Version: 2.1
-Name: iql
-Version: 0.1.6
-Summary: SQL Overlay Language with support for Bloomberg BQL, FRED, Edgar, Kaggle and other financial data sources within SQL
-Home-page: https://www.iqmo.com
-Author: Paul Timmins
-Author-email: paul@iqmo.com
-Keywords: IQMO Query Language IQMOQL BQL BQUANT FRED EDGAR KAGGLE
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: duckdb (>=0.7.0)
-Requires-Dist: pandas (>=1.3.4)
-Requires-Dist: sqlparse (>=0.4.3)
-
-# IQMO Query Language (IQL)
-
-IQL extends SQL with pluggable Python extensions allowing you to use external data seamlessly within SQL. It's intended as a light weight layer to allow insertion of code, all fully within SQL. IQL provides extensions for a variety of data sources: 
-
-IQL works out of the box, allowing you to execute SQL statements over your dataframes and external data sources with no configuration. It is able to do this because of DuckDB, IQL's default database, but other databases may also be connected/used. DuckDB is a highly performant in-memory OLAP database: it's great for complex analytical work. 
-
-- SEC EDGAR
-    ```
-    iql.execute(f"select * from edgar(type='submissions', cik='{CIK}')")
-    ```
-- Bloomberg Query Language (BQL)
-    ```
-    iql.execute(f"""select * from bql("{bqlquery}") as bql1 join mytable on mytable.id=bql1.id""")
-    ```
-- Kaggle Data Files
-    ```
-    iql.execute(f"""select * from kaggle("user/dataset/datafile")""")
-    ```
-- FRED Economic Data
-    ```
-    iql.execute(f"""select * from fred(type="observations", seriesid="{seriesid}", startdate="{date_str}") as freddata""")
-    ```
-- Pandas operations
-    ```
-    SELECT * FROM pandas(table=xyz, pivot=('col1', 'col2', 'values'))
-    ```
-
-## Why?
-IQL allows many analytics tasks to be condensed into simpler queries, and allows seamless interplay between Pandas (or Polars) dataframes and database operations. 
-
-SQL (with IQL) condenses a lot of tedious and repetitive Pandas code and is friendlier to non-developers who don't need to learn the intricacies of the Pandas API.
-
-We use IQL for early stage exploration, cleaning and staging. We also use IQL for later stage reporting and data presentation. In between, we still use Pandas/Polars for intermediate ML and modelling. 
-
-### Native Formats
-Our goal is to support the native formats of the systems:
-- The native SQL of the database engine is supported: only the IQL SubQuery's are used. 
-- The native SubQuery syntax is preserved. Bloomberg BQL queries run without modification. REST API calls can be called via URLs directly. etc.
-
-### Simplicity and Performance
-Multiple transformations, aggregations and operations can be expressed in a single statement. This reduces the amount of code we need to write, eliminates long chains of Pandas operations, and often leads to significant performance increases. 
-
-IQL's default database is a higly efficient in-memory OLAP database called DuckDB. [DuckDB Performance vs Pandas](https://duckdb.org/2021/05/14/sql-on-pandas.html)
-
-### All in One Place and Extensible
-
-You can query REST APIs as if they were database tables. You can add custom business logic to control how certain files are retrieved, cached or pre-processed.
-
-IQL is portable across DB environments. DuckDB is shipped by default, but can be replaced with PyArrow, SnowFlake or other databases.
-
-### How Does It Work
-How does it work? IQL iterates over SQL statements (if multiple statements are used), and extracts IQL SubQuerys (ie: fred(...)). Each SubQuery is executed and stored (as a DataFrame or local file). The SQL query is modified to reference the results of the SubQuery instead of the SubQuery itself, and the database engine runs the modified SQL query. 
-
-For example, given the following query:
-```  
-SELECT * 
-  FROM fred('query1') as q1
-  JOIN fred('query2') as q2
-      ON q1.id=q2.id
-```
-In pseudocode (this is logically but not literally what happens):
-```
-  # pseudocode
-  df_q1 = iql.execute("fred('query1")")
-  df_q2 = iql.execute("fred('query2")")
-
-  db.execute("SELECT * FROM df_q1 JOIN df_q2 on df_q1.id = df_q2.id")
-```
-
-## Disclaimers
-
-READ the license. We do not WARRANTY this for anything. This software is provided AS IS. TEST before you use. Use at your OWN risk. ETC.
-
-THIS PROJECT IS NOT AFFILIATED WITH, SUPPORTED BY, ENDORSED BY OR CONNECTED TO ANY OF THE COMPANIES, PRODUCTS OR SERVICES BELOW.
-
-
-# Extensions:
-
-- [Bloomberg BQL](BLOOMBERG_BQL_README.md)
-- [Kaggle Datasets](https://www.kaggle.com/datasets)
-  - Requires kaggle module
-    pip install kaggle
-- [FRED Economic Data](https://fred.stlouisfed.org/docs/api/fred/)
-- [Amazon S3](https://aws.amazon.com/s3/): S3 API extension will download Parquet and CSV files locally, and then access them via DuckDB's Parquet and CSV support.
-  - Requires boto3
-    pip install boto3
-  - Alternatively, use DuckDBs [HTTPFS](https://duckdb.org/docs/extensions/httpfs.html) to access S3.
-  - The IQL AWS extension provides a caching, authentication and logic entrypoint
-  - The DuckDB extension provides support for processing multiple Parquet files, such as with Hive partitions.
-  - More information on [DuckDB and Parquet](https://duckdb.org/docs/data/parquet)
-- [Pandas](https://pandas.pydata.org/): Allows Pandas operations to be executed within the SQL statement. Not all Pandas operations are available.
-
-See the examples/ folder for complete examples.
-
-## Syntax
-
-IQL extensions are executed as functional subqueries. Each extension is registered with a unique name.
-
-Kaggle:
-
-```
-SELECT \*
-FROM
-kaggle('username/datasetname/filename')
-```
-
-or (FRED and Kaggle)
-
-```
-SELECT \*
-FROM
-kaggle("....") q1
-JOIN
-fred("....") q2
-ON
-q1.something = q2.something
-```
-
-or (Bloomberg BQL)
-
-```
-SELECT \*
-FROM
-bql("get (...) for (...)") q1
-JOIN
-bql("get (...) for (...)") q2
-ON
-q1.id = q2.id
-```
-
-See the example notebooks for more interesting examples.
-
-## Dependencies
-
-- Extensions may have specific module dependencies, such as the Kaggle Extensions requiring the Kaggle API.
-- Extensions are loaded dynamically on first use, so dependencies are not required at install time
-- duckdb is required, although not needed if a different db_connector is used.
-
-## SQL Syntax
-
-IQL does not modify the SQL other than replacing the underlying SQL.
-
-See the database specific documentation for more information: [DuckDB SQL Statements](https://duckdb.org/docs/sql/introduction)
-
-## Quoting Strings
-
-Strings must be properly quoted and/or escaped, according to normal Python rules. The SubQuery requires a quoted string, be careful to use different quote types for the entire SQL string and the SubQuery string.
-
-It's not that complicated, but it's easy to screw up with multiple levels of quoting.
-
-Triple quotes are convenient, since SQL queries tend to be long and multi-line. Note the three levels of quotes: triple """, single " and single '.
-
-```
-import iql
-
-bql_str = "get (...) for ('XYZ')"
-sql_str = f"""
-    -- This uses a Python f-string, which allows us to use the {bql_str} variable
-    SELECT *
-    FROM
-        -- bql() is an IQL extension. Note the quotes around the BQL statement.
-        -- if the BQL statement contains double quotes,
-        bql("{bql_str}")
-    """
-
-iql.execute(sql_str)
-```
-
-Or, make sure to escape properly, such as here:
-
-```
-import iql # Use \" to escape the double quotes within double quotes
-iql.execute("SELECT \* FROM bql('get (...) for (\"XYZ\")')")
-```
-
-Sometimes it's just easier to break a query into smaller strings.
-
-```
-import iql
-bql_str = "get (...) for ('XYZ')"
-iql.execute(f"""
-    SELECT *
-    FROM
-    bql("{BQL}")
-  """)
-```
-
-# Getting Started - Kaggle
-
-## Authentication - KAGGLE_KEY and KAGGLE_USERNAME
-
-Login to Kaggle and visit the account page to download the configuration JSON. Extract the KEY and USERNAME from the configuration JSON.
-
-Set KAGGLE_KEY and KAGGLE_USERNAME to the appropriate values, or set it via:
-
-```
-from iql.extensions import kaggle_extension
-kaggle_extension.set_kaggle_credentials(kaggle_username='your username', kaggle_key='kaggle API key')
-```
-
-## Usage
-
-SubQuery syntax is:
-
-```
-kaggle("{user}/{dataset}/{filename}")
-```
-
-Example:
-
-```
-import iql
-iql.execute('SELECT \* FROM kaggle("{user}/{dataset}/{filename}")')
-```
-
-Currently, only CSV and XLSX datasets are supported. See examples/kaggle_examples.ipynb notebook for more complete examples.
-
-## Comments
-
-The Kaggle extension will download the file once and reuse it as long as it's in the local directory. This will persist across kernel restarts. You can override this behavior by passing the refreshcache=True flag:
-
-```
-iql.execute('SELECT * FROM kaggle("{user}/{dataset}/{filename}", refreshcache=True)')
-```
-
-The Kaggle extension will also load the datafile to an in-memory DataFrame. In our testing, the extension was slower for the first read than DuckDB's read_csv_auto, but subsequent reuse was subsequently much faster. The extension could be modified to download the file and use DuckDB's read_csv_auto feature instead of creating a DataFrame (similar to the AWS S3 Extension). In our testing, our in-memory approach was faster for analytical workloads with ample memory and frequent reuse.
-
-# Pandas Extension
-
-The pandas options are available in every extension, but sometimes its better to run after the data has been first populated in an earlier query.
-
-The syntax is:
-
-```
-iql.execute("""SELECT \* FROM pandas(table=xyz, pivot=('col1', 'col2', 'values'))"""
-```
-
-These operations may also be used in each of the extensions:
-
-- fillna_pre='string': Before pivoting, replaces only in a single column: DataFrame["value"].fillna(val)
-- dropna_pre=True | str | list[str]: Before pivoting, If True, DataFrame.dropna(). Else, DataFrame.dropna(subset=[value])
-- pivot=(index,columns,values): DataFrame.pivot(index=index, columns=columns, values=values)
-- fillna=val: DataFrame.fillna(val)
-- dropna=True | str | list[str]: If True, DataFrame.dropna(). Else, DataFrame.dropna(subset=[value])
-
-Note: While still in development, [DuckDB's Pivot and Unpivot](https://github.com/duckdb/duckdb/pull/6387) may change how we handle pivoting.
-
-# Operations available to all IQL SubQueries:
-
-## Parameter Passing
-
-There are two ways to dynamically pass parameters:
-
-- Fixed List: A list of fixed parameters may be passed. In this example, the paramlist is evaluated first, and any occurence of $SERIESID in the entire fred() option is replaced. One query is run for each value, and the results are UNIONed.
-
-```
-query2 = f"""select * from fred(type="series", seriesid="$SERIESID", paramlist=("$SERIESID", ["UNRATE", "EXUSEU"])) as q1"""
-```
-
-- Dynamic Lists: A list of values from a previous run query may also be passed. In this example, a list of values is created in the first query, then for each value, a FRED function is called and the results are UNIONed
-
-```
-# Using a parameter list to retrieve multiple series
-# SQL uses single quotes for string literals / constants. Unlike Python, SQL treats single and double quotes differently.
-
-query2 = f"""
-    CREATE TEMP TABLE series_results as values('UNRATE'), ('EXUSEU');
-    SELECT * FROM fred(type="series", seriesid="$SERIESID", paramquery=("$SERIESID", "select * from series_results")) as q1
-    """
-df2 = iql.execute(query2)
-display(df2)
-```
-
-Limitations: Only one paramquery or paramlist may be used per SubQuery.
-
-# Getting Started - FRED Economic Data
-
-The FRED extension is a lightweight wrapper around [FRED's REST API](https://fred.stlouisfed.org/docs/api/fred/)
-
-We opted to not build yet another parameterized / Pythonic API for FRED. Instead, we use the native REST URLs as the query parameters.
-
-Instead, just find a REST endpoint want, construct a query string, and query it natively.
-
-## Get a FRED FRED_API_KEY
-
-Visit [FRED](https://fred.stlouisfed.org/) and create an account and get your API key.
-
-## Set the API Key
-
-```
-from iql.extensions import fred_extension
-fred_extension.FRED_API_KEY = abcdef
-```
-
-## Usage: Types
-
-Releases, Series and Observations
-
-```
-query1 = """select \* from fred(type="releases")"""
-
-seriesid = "UNRATE"
-query2 = f"""select * from fred(type="series", seriesid="{seriesid}") as q1"""
-
-seriesid = "UNRATE"
-date_str = "2023-01-01"
-query3 = f"""select * from fred(type="observations", seriesid="{seriesid}", startdate="{date_str}") as q1"""
-```
-
-## Usage: Raw URL
-
-```
-"""Get information about a FRED series"""
-seriesid = "UNRATE"
-query = f"SELECT * FROM fred('https://api.stlouisfed.org/fred/series?series_id={seriesid}') as q1"
-df = iql.execute(query)
-display(df)
-```
-
-See the exammples/fred_examples.ipynb notebook for examples.
-
-# IQL extension for Bloomberg BQL
-
-See [IQL Extension for Bloomberg BQL Readme](BLOOMBERG_BQL_README.md) for more information.
-
-## Amazon S3 Extension
-
-The Amazon S3 extension downloads Parquet and CSV files directly from S3 to a local file, then uses DuckDBs native support to access the local Parquet and CSV files.
-
-We implemented this to add our own authentication and caching logic to reduce frequent downloads of the same data.
-
-## Troubleshooting: If you see an initialization failure, verify that BQL is available and working.
-
-```
-import bql
-bq = bql.Service()
-bq.execute("get(name) for('IBM US Equity')")
-```
-
-If this fails, you are probably not running in BQuant.
-
-# AWS S3 Extension
-
-IQL provides an S3 Extension to provide an entrypoint for control of S3 data retrieval and local caching. This extension is intended to be extended to support environment-specific authentication and cache control requirments.
-
-Usage:
-
-```
-SELECT * FROM s3('s3://bucket/prefix/key/objname.parquet') as data1
-```
-
-What happens:
-
-- objname.parquet is to the iql.iqmo.DEFAULT_EXT_DIRECTORY, or the default dir if no directory is set.
-- s3(...) is replaced with a reference to the local Parquet file, allowing the database engine to read the Parquet file natively
-
-## S3 File Caching
-
-S3 files are downloaded locally and reused while the cache reference has not expired.
-
-## AWS Authentication
-
-- Default behavior: The AWS S3 extension simply calls - boto3.resource("s3"), assuming the environment is already set properly
-- Option 1: Create and store boto3 S3 resources to iql.extensions.aws_s3_extension::BOTO_S3_RESOURCES for each bucket
-
-```
-from iql.extensions import aws_s3_extension
-url_prefix = "s3://something/something"
-.... AWS CREDENTIAL STUFF ....
-s3res = boto3.resource("s3")
-aws_s3_extension.BOTO3_S3_RESOURCES[url_prefix] = s3res
-```
-
-- Option 2: Replace iql.extensions.aws_s3_extension::get_boto3_resource_for_request(), which takes a single URL parameter and returns a boto3 resource object
-
-# Caching
-
-SubQueries are often expensive and often reused while developing and refining queries. If enabled, IQL will cache the SubQuery results in memory and/or in a persistent file cache.
-
-Caching can be controlled via activate_cache:
-
-```
-def activate_cache(duration_seconds: Optional[int], cache_directory: Optional[str]):
-```
-
-duration_seconds:
-
-```
--1 (Default): Infinite (for life of kernel)
-None: Disabled
-int: Maximum life of the cached value from the time of creation.
-```
-
-cache_directory:
-
-```
-None (Default): Don't use a persistent file cache
-path: Location for the external file cache
-```
-
-## Caching Waterfall
-
-- nocache directive
-- cache directive
-- extension cache period
-- global \_CACHE_PERIOD
-
-## Caching Limitations
-
-Cached values are not pruned on expiration. The in memory dictionary is cleared on kernel restart. The file cache will grow unbounded until cleared:
-
-```
-from iql import q_cache # clear the in memory and file cache
-xq_cache.clear_caches()
-```
-
-## Caching Hints
-
-### cache=seconds
-
-Overrides the caching period. -1 is infinite caching.
-
-```
-iql.execute("""SELECT * FROM keyword("...", cache=60) as q1""")
-```
-
-### nocache=True
-
-Does not use any cached results
-
-```
-iql.execute("""SELECT * FROM keyword("...", nocache=True) as q1""")
-```
-
-## Caching Best Practices
-
-Caching is important to get right but depend on the data and use cache. Caching can significantly improve performance during design and development which frequently reuse unchanging data. For live data that changes frequently, an appropriate cache interval should be used to avoid reuse of stale data.
-
-If your kernels are short-lived, this is largely a non-issue, since the cache is reset automatically, unless a file cache is activated.
-
-# Database
-
-## Valid Queries
-
-In DuckDB, IQL was developed against DuckDB's statements, including SELECTs with CTE's (WITH clauses). IQL is seamless: it only modifies the extension SubQueries, and otherwise passes the results to the database.
-
-Any valid DuckDB query should be supported.
-
-When troubleshooting, check the usual suspects first:
-
-- Make sure parentheses and quotes are balanced
-  Most query errors are from forgetting a closing quote and/or parenthesis.
-- SQL uses single quotes for string literals (constants):
-
-```
-  select 'abc' # 'abc' is a string literal
-```
-
-is not the same as
-
-```
-select "abc" # "abc" is a column name
-```
-
-- Valid SQL syntax: Complex SQL queries can be cumbersome. Consider breaking a complex query into several individual steps, at least to refine the logic. This can have a negative performance impact as it defeats any database query optimization, but in practical terms, it is often beneficial.
-
-## Database Lifecycle
-
-### Default: In-Memory Database for each iql.execute()
-
-By default, a series of iql.execute() calls will create and close an in-memory DuckDB connection for each request. 
-
-### Option 1: Keep Database Open
-
-Use the iql default connection setting (in-memory only), but leave the connection open:
-
-```
-con = iql.IQL.get_dbconnector().get_connection()
-try:
-  iql.execute("CREATE TABLE abc as SELECT * FROM (values(1),(2),(3))", con=con)
-  df=iql.execute("SELECT * FROM abc", con=con)
-  display(df)
-finally:
-  con.close()
-```
-
-SQL statements separated by semicolons. The entire set will be run sequentially against a single database, so side effects will be maintained.
-
-### Option 2: Create Database Externally
-
-With this method, you can use a file-based persistent database along with other connectivity options.
-
-Or, create a DuckDB Connection [duckdb.connect()](https://duckdb.org/docs/api/python/overview), such as for a file-based persistent database.
-
-```
-df=iql.execute("SELECT * FROM abc", con=con)
-```
-
-# FAQ
-
-## Why DuckDB as the default?
-
-We chose [DuckDB](https://duckdb.org/) as the default database module for a few reasons:
-
-- DuckDB is awesome and [fast](https://duckdb.org/2021/05/14/sql-on-pandas.html), with vectorized columnar operations.
-- It runs with no setup
-- It runs fully locally and has support for a variety of data sources
-- DuckDB's SQL language is standard
-- DuckDB natively supports Pandas
-
-## Why not a DuckDB Extensions?
-
-We could have written this as a set of DuckDB extensions, but we didn't. Why?
-
-- Portability: DuckDB is great, but it's not the only game in town. PyArrow and SnowFlake are important.
-- Native Python is easy to develop, easy to debug, and convenient to modify and extend.
-- Performance: In our workflows, there was little performance to be gained. Runtime was dominated by external data transfer.
-
-## Databases other than DuckDB:
-
-Any database can be supported by implementing a database module. The key step that's dependent on the database engine is registering (or loading) the SubQuery dataframes to the database engine prior to executing the queries.
-
-Modules could be added to support other databases:
-
-- [SQLDF](https://pypi.org/project/sqldf/) and [PandaSQL](https://pypi.org/project/pandasql/): Local-only databases that can connect to in-memory Pandas dataframes
-- PyArrow: SubQuery dataframes would be loaded via [pyarrow.Table.from_pandas()](https://arrow.apache.org/docs/python/pandas.html)
-- SnowFlake: During registration step, the Pandas dataframes need to be loaded via the [SnowFlake Pandas Connector](https://docs.snowflake.com/en/user-guide/python-connector-pandas)
-- Other Pandas-centric engines, such as SQLDF and PandaSQL
-
-## What about Polars?
-
-Since DuckDB supports Polars, IQL extensions could be modified to use Polars DataFrames since DuckDB supports Polars. This would be a relatively simple change, made in each extension to create a Polars DataFrame instead of a Pandas DataFrame. This could be made extensible, so the default DataFrame implementation is user selectable.
-
-## Design Principles
-
-- Extensibility: Extensions and Database Connectors can be easily modified, replaced, or extended.
-- KISS: Keep it simple. Don't add complexity.
-  - REST APIs, such as FRED: Use the complete URL, rather than building yet-another-Python-API
-  - Bloomberg BQL: Use native BQL queries without modification
-- Minimal dependencies: Extensions are loaded on-demand. Unused dependencies are not required.
-
-# Footnotes
-
-## Useful DuckDB Features
-
-### CTEs
-
-```
-import iql
-df = iql.execute("""
-  WITH c AS keyword("..."),
-      idx AS keyword("...")
-    SELECT c.*, idx.*
-    FROM c
-    JOIN idx
-      ON c.idx=idx.id""")
-display(df)
-```
-
-### Accessing Global DataFrames:
-
-```
-import iql
-import pandas as pd
-
-fun = pd.DataFrame([{'id': 'Someone', 'fun_level': 'High'}])
-iql.execute("""SELECT * FROM fun""")
-```
-
-### Copy (query) to 'file'
-
-```
-import iql
-iql.execute("""COPY (query) TO 'somefile.parquet'""")
-```
-
-## Copy to Paruet
-
-- Copy to parquet:
-  https://duckdb.org/docs/guides/import/parquet_export.html#:~:text=To%20export%20the%20data%20from,exported%20to%20a%20Parquet%20file.
-
-# Futures
-
-## SQL ReWrite
-Instead of modifying the SQL in a single step, we could introduce an intermediate statement that has the same logical flow as the code today. This would make it easier to debug, allowing the user to view and debug each step. 
-```
-SELECT * FROM fred() a JOIN fred() b on a.id=b.id
-```
-could be transformed first into:
-```
-a=fred();
-b=fred();
-SELECT * FROM a JOIN b
-```
-
-One decision needed here is how to express the first two statements: would we use a CREATE TEMP TABLE or COPY TO to store the SubQuery results, or do we introduce something like CREATE DF.  
-
-## Simplifying Parsing
-
-We didn't implement a grammar, because each grammar is very platform dependent. Each database has its own product-specific grammar. 
-
-The current IQL implementation first parses the SQL to extract the named functions, using the sqlparse library, then extracts the IQL subquerys by their named keywords. The SubQueries are then parsed via an AST to extract the parameters and values. Any parsing introduces risks and fragility:  
-- It's possible that sqlparse will fail to parse certain database specific language features. We haven't encountered this yet, but it's something we're thinking about
-- It's also possible that our extraction will fail to recognize proper subqueries, due to how sqlparse extracts the tokens. The code here is not as robust as we'd like, and more testing is needed.
-
-There's a few ways to improve this:
-- Direct string extraction: identify subquery() blocks and extract them directly as strings, rather than parsing the entire SQL file. This would have to properly account for commenting, quoting, and nesting.
-- DuckDB (or whatever platform) extensions: use a lightweight extension to allow the database to externally call the IQL layer, rather than having IQL act as an intermediate step.
-
-## Caching
-The in-memory cache will grow unbounded within each kernel session. The expiration is only used to invalid data, but expired results are not evicted from memory if not accessed. 
-
-We'll replace the in-memory cache with something more robust, probably another cache implementation such as [cachetools](https://github.com/tkem/cachetools). Alternatively, IQL could maintain a cache per "session", rather than globally.
-
-If your kernels are long-lived, clear the cache at appropriate intervals or points in your workflow:
-
-```
-iql.clear_caches()
-```
-
-## Parquet Files or PyArrow vs DataFrame
-
-In-Memory Extensions could serialize data to other formats, instead of to DataFrames. 
-
-Note: This isn't required for file-based extensions like AWS S3. 
-
-## Projection and Filter Pushdowns
-
-SubQueries are executed in their entirety _first_ and then queried by the database.
-
-This could be modified to add support for projection and filter pushdowns, similar to what was done in the [DuckDB - Querying Parquet](https://duckdb.org/2021/06/25/querying-parquet.html).
-
-The main concern here is both complexity and dependency on database specifics. Currently, paramquery's provide a similar (but more limited) benefit with little added complexity.
-
-## Limitations
-
-SubQueries are executed in their entirety, so a SubQuery cannot be parameterized based on results from another SubQuery without using an intermediate table: execute the first SubQuery, store the results in a table, then execute the second SubQuery with a paramquery.
-
-# Footer
-
-Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
-All Rights Reserved
+Metadata-Version: 2.1
+Name: iql
+Version: 0.1.9b5
+Summary: SQL Overlay Language with support for Bloomberg BQL, FRED, Edgar, Kaggle and other financial data sources within SQL
+Home-page: https://github.com/iqmo-org/iql_dev
+Author: Paul Timmins
+Author-email: paul@iqmo.com
+Keywords: IQMO Query Language IQMOQL BQL BQUANT FRED EDGAR KAGGLE
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: duckdb (>=0.7.1)
+Requires-Dist: pandas (>=1.5.3)
+Requires-Dist: sqlparse (>=0.4.3)
+Requires-Dist: pyarrow
+
+# Intermediate Query Language (IQL)
+
+IQL is a framework and a collection of Python-based extensions for financial data acquisition.
+
+# Installation
+
+```
+# Install
+%pip install iql --upgrade
+
+# Load Magics to enable %iql and %%iql for VScode and Jupyter
+%load_ext iql.jupyter_magics.iql_magic
+```
+
+# Usage
+
+Python API
+
+```
+import iql
+df1 = iql.execute(f"select * from ...")
+```
+
+Cell Magic
+
+```
+%%iql -o df1
+select * from ...
+```
+
+Line Magic
+
+```
+df1 = %iql select * from ...
+```
+
+# About IQL
+
+IQL serves two purposes: a framework for adding lightweight extensions to data pipelines through declarative SQL queries, and a collection of useful extensions.
+
+## IQL: The Framework
+
+IQL allows python functions to be registered and executed inline with SQL. These functions take parameters and can return DataFrames, Parquet Files, or CSVs.
+
+```
+SELECT * FROM myextension(param='abc', param2='def')
+```
+
+In this simple example, IQL extracts and preprocesses myextension. The SQL is rewritten to replace myextension, and the DataFrame is registered with the database. The exact mechanism depends on the database: for DuckDB (default database), the dataframes can be queried on the fly without loading explicitly to the database.
+
+## IQL: The Extensions
+
+IQL works out of the box, allowing you to execute SQL statements over your dataframes and external data sources with no configuration.
+
+- SEC EDGAR
+
+  `%iql select * from edgar(type='submissions', cik='{CIK}')`
+
+- Bloomberg Query Language (BQL)
+
+  `%iql select * from bql("get(px_last) for(['IBM US Equity']) with(dates=range(-90D, 0D), fill=prev)") order by value desc limit 3`
+
+- Kaggle
+
+  `iql.execute(f"""select * from kaggle("user/dataset/datafile")""")`
+
+- FRED Economic Data
+
+  `iql.execute(f"""select * from fred(type="observations", seriesid="{seriesid}", startdate="{date_str}") as freddata""")`
+
+- Pandas operations
+
+  `SELECT * FROM pandas(table=xyz, pivot=('col1', 'col2', 'values'))`
+
+- Machine Learning: SKLearn and XGBoost
+
+## Why?
+
+SQL is a powerful declarative language, capable of expressing complex data manipulations and enabling efficient optimized processing. Often, interaction with external data is required, making it difficult to build interactive systems leveraging declarative data structures. Combining SQL with a pre-processing framework to externalize data load within the context of a SQL query makes many workflows simpler.
+
+Modern analytical databases, such as [DuckDB](https://github.com/duckdb), provide many powerful tools to allow more to be done within SQL and eliminating the back and forth required for data loading and manipulation. IQL is intended to extend the power of these platforms without being tied to a single platform: through the use of pre-processed extensions.
+
+### Native Formats
+
+After preprocessing of the IQL Extension queries, the database engine will execute a native query unmodified. This minimizes the dependency on specific databases and database versions.
+
+The native SQL format of the database engine is supported: the SQL runs unmodified except for replacement of the IQL SubQueries.
+
+The native SubQuery syntax is preserved. Bloomberg BQL queries run without modification. REST API calls can be called via URLs directly. etc.
+
+### Simplicity and Performance
+
+Multiple transformations, aggregations and operations can be expressed in a single statement. This reduces the amount of code we need to write, eliminates long chains of Pandas operations, and often leads to significant performance increases.
+
+IQL's default database is a higly efficient in-memory OLAP database called DuckDB, which requires zero configuration or administration. You may use a transient database per query, or create a long-lived database and reuse across queries. [DuckDB Performance vs Pandas](https://duckdb.org/2021/05/14/sql-on-pandas.html)
+
+### All in One Place and Extensible
+
+You can query REST APIs as if they were database tables. You can add custom business logic to control how certain files are retrieved, cached or pre-processed.
+
+IQL is portable across DB environments. DuckDB is shipped by default, but can be replaced by other databases.
+
+### How Does It Work
+
+How does it work? IQL iterates over SQL statements (if multiple statements are used), and extracts IQL SubQuerys (ie: fred(...)). Each SubQuery is executed and stored (as a DataFrame or local file). The SQL query is modified to reference the results of the SubQuery instead of the SubQuery itself, and the database engine runs the modified SQL query.
+
+For example, given the following query:
+
+```
+%%iql
+SELECT *
+  FROM fred('query1') as q1
+  JOIN fred('query2') as q2
+      ON q1.id=q2.id
+```
+
+In pseudocode (this is logically but not literally what happens):
+
+```
+  # pseudocode
+  df_q1 = iql.execute("fred('query1")")
+  df_q2 = iql.execute("fred('query2")")
+
+  db.execute("SELECT * FROM df_q1 JOIN df_q2 on df_q1.id = df_q2.id")
+```
+
+Or, using the %iql cell magic:
+
+## Disclaimers
+
+READ the license. We do not WARRANTY this for anything. This software is provided AS IS. TEST before you use. Use at your OWN risk. ETC.
+
+THIS PROJECT IS NOT AFFILIATED WITH, SUPPORTED BY, ENDORSED BY OR CONNECTED TO ANY OF THE COMPANIES, PRODUCTS OR SERVICES BELOW.
+
+# Extensions:
+
+- [Bloomberg BQL](BLOOMBERG_BQL_README.md)
+- [Kaggle Datasets](https://www.kaggle.com/datasets)
+  - Requires kaggle module
+    pip install kaggle
+- [FRED Economic Data](https://fred.stlouisfed.org/docs/api/fred/)
+- [Amazon S3](https://aws.amazon.com/s3/): S3 API extension will download Parquet and CSV files locally, and then access them via DuckDB's Parquet and CSV support.
+  - Requires boto3
+    pip install boto3
+  - Alternatively, use DuckDBs [HTTPFS](https://duckdb.org/docs/extensions/httpfs.html) to access S3.
+  - The IQL AWS extension provides a caching, authentication and logic entrypoint
+  - The DuckDB extension provides support for processing multiple Parquet files, such as with Hive partitions.
+  - More information on [DuckDB and Parquet](https://duckdb.org/docs/data/parquet)
+- [Pandas](https://pandas.pydata.org/): Allows Pandas operations to be executed within the SQL statement. Not all Pandas operations are available.
+
+See the examples/ folder for complete examples.
+
+## Syntax
+
+IQL extensions are executed as functional subqueries. Each extension is registered with a unique name.
+
+Kaggle:
+
+```
+SELECT \*
+FROM
+kaggle('username/datasetname/filename')
+```
+
+or (FRED and Kaggle)
+
+```
+SELECT \*
+FROM
+kaggle("....") q1
+JOIN
+fred("....") q2
+ON
+q1.something = q2.something
+```
+
+or (Bloomberg BQL)
+
+```
+SELECT \*
+FROM
+bql("get (...) for (...)") q1
+JOIN
+bql("get (...) for (...)") q2
+ON
+q1.id = q2.id
+```
+
+See the example notebooks for more interesting examples.
+
+## Dependencies
+
+- Extensions may have specific module dependencies, such as the Kaggle Extensions requiring the Kaggle API.
+- Extensions are loaded dynamically on first use, so dependencies are not required at install time
+- duckdb is required, although not needed if a different db_connector is used.
+
+## SQL Syntax
+
+IQL does not modify the SQL other than replacing the underlying SQL.
+
+See the database specific documentation for more information: [DuckDB SQL Statements](https://duckdb.org/docs/sql/introduction)
+
+## Quoting Strings
+
+Strings must be properly quoted and/or escaped, according to normal Python rules. The SubQuery requires a quoted string, be careful to use different quote types for the entire SQL string and the SubQuery string.
+
+Triple quotes are convenient, since SQL queries tend to be long and multi-line. Note the three levels of quotes: triple """, single " and single '.
+
+```
+import iql
+
+bql_str = "get (...) for ('XYZ')"
+sql_str = f"""
+    -- This uses a Python f-string, which allows us to use the {bql_str} variable
+    SELECT *
+    FROM
+        -- bql() is an IQL extension. Note the quotes around the BQL statement.
+        -- if the BQL statement contains double quotes,
+        bql("{bql_str}")
+    """
+
+iql.execute(sql_str)
+```
+
+In Notebooks, this is a little simpler, since the outer quotes aren't needed:
+
+```
+%%iql -o bql_df
+
+SELECT * FROM bql("get(px_last) for ([`IBM US Equity`])")
+```
+
+# Getting Started - Kaggle
+
+## Authentication - KAGGLE_KEY and KAGGLE_USERNAME
+
+Login to Kaggle and visit the account page to download the configuration JSON. Extract the KEY and USERNAME from the configuration JSON.
+
+Set KAGGLE_KEY and KAGGLE_USERNAME to the appropriate values, or set it via:
+
+```
+from iql.extensions import kaggle_extension
+kaggle_extension.set_kaggle_credentials(kaggle_username='your username', kaggle_key='kaggle API key')
+```
+
+## Usage
+
+SubQuery syntax is:
+
+```
+kaggle("{user}/{dataset}/{filename}")
+```
+
+Example:
+
+```
+import iql
+iql.execute('SELECT \* FROM kaggle("{user}/{dataset}/{filename}")')
+```
+
+Currently, only CSV and XLSX datasets are supported. See examples/kaggle_examples.ipynb notebook for more complete examples.
+
+## Comments
+
+The Kaggle extension will download the file once and reuse it as long as it's in the local directory. This will persist across kernel restarts. You can override this behavior by passing the refreshcache=True flag:
+
+```
+iql.execute('SELECT * FROM kaggle("{user}/{dataset}/{filename}", refreshcache=True)')
+```
+
+The Kaggle extension will also load the datafile to an in-memory DataFrame. In our testing, the extension was slower for the first read than DuckDB's read_csv_auto, but subsequent reuse was subsequently much faster. The extension could be modified to download the file and use DuckDB's read_csv_auto feature instead of creating a DataFrame (similar to the AWS S3 Extension). In our testing, our in-memory approach was faster for analytical workloads with ample memory and frequent reuse.
+
+# Pandas Extension
+
+The pandas options are available in every extension, but sometimes its better to run after the data has been first populated in an earlier query.
+
+The syntax is:
+
+```
+iql.execute("""SELECT \* FROM pandas(table=xyz, pivot=('col1', 'col2', 'values'))"""
+```
+
+These operations may also be used in each of the extensions:
+
+- fillna_pre='string': Before pivoting, replaces only in a single column: DataFrame["value"].fillna(val)
+- dropna_pre=True | str | list[str]: Before pivoting, If True, DataFrame.dropna(). Else, DataFrame.dropna(subset=[value])
+- pivot=(index,columns,values): DataFrame.pivot(index=index, columns=columns, values=values)
+- fillna=val: DataFrame.fillna(val)
+- dropna=True | str | list[str]: If True, DataFrame.dropna(). Else, DataFrame.dropna(subset=[value])
+
+Note: While still in development, [DuckDB's Pivot and Unpivot](https://github.com/duckdb/duckdb/pull/6387) may change how we handle pivoting.
+
+# Operations available to all IQL SubQueries:
+
+## Parameter Passing
+
+There are two ways to dynamically pass parameters:
+
+- Fixed List: A list of fixed parameters may be passed. In this example, the paramlist is evaluated first, and any occurence of $SERIESID in the entire fred() option is replaced. One query is run for each value, and the results are UNIONed.
+
+```
+query2 = f"""select * from fred(type="series", seriesid="$SERIESID", paramlist=("$SERIESID", ["UNRATE", "EXUSEU"])) as q1"""
+```
+
+- Dynamic Lists: A list of values from a previous run query may also be passed. In this example, a list of values is created in the first query, then for each value, a FRED function is called and the results are UNIONed
+
+```
+# Using a parameter list to retrieve multiple series
+# SQL uses single quotes for string literals / constants. Unlike Python, SQL treats single and double quotes differently.
+
+query2 = f"""
+    CREATE TEMP TABLE series_results as values('UNRATE'), ('EXUSEU');
+    SELECT * FROM fred(type="series", seriesid="$SERIESID", paramquery=("$SERIESID", "select * from series_results")) as q1
+    """
+df2 = iql.execute(query2)
+display(df2)
+```
+
+Limitations: Only one paramquery or paramlist may be used per SubQuery.
+
+# Getting Started - FRED Economic Data
+
+The FRED extension is a lightweight wrapper around [FRED's REST API](https://fred.stlouisfed.org/docs/api/fred/)
+
+We opted to not build yet another parameterized / Pythonic API for FRED. Instead, we use the native REST URLs as the query parameters.
+
+Instead, just find a REST endpoint want, construct a query string, and query it natively.
+
+## Get a FRED FRED_API_KEY
+
+Visit [FRED](https://fred.stlouisfed.org/) and create an account and get your API key.
+
+## Set the API Key
+
+```
+from iql.extensions import fred_extension
+fred_extension.FRED_API_KEY = abcdef
+```
+
+## Usage: Types
+
+Releases, Series and Observations
+
+```
+query1 = """select \* from fred(type="releases")"""
+
+seriesid = "UNRATE"
+query2 = f"""select * from fred(type="series", seriesid="{seriesid}") as q1"""
+
+seriesid = "UNRATE"
+date_str = "2023-01-01"
+query3 = f"""select * from fred(type="observations", seriesid="{seriesid}", startdate="{date_str}") as q1"""
+```
+
+## Usage: Raw URL
+
+```
+"""Get information about a FRED series"""
+seriesid = "UNRATE"
+query = f"SELECT * FROM fred('https://api.stlouisfed.org/fred/series?series_id={seriesid}') as q1"
+df = iql.execute(query)
+display(df)
+```
+
+See the exammples/fred_examples.ipynb notebook for examples.
+
+# IQL extension for Bloomberg BQL
+
+See [IQL Extension for Bloomberg BQL Readme](BLOOMBERG_BQL_README.md) for more information.
+
+## Amazon S3 Extension
+
+The Amazon S3 extension downloads Parquet and CSV files directly from S3 to a local file, then uses DuckDBs native support to access the local Parquet and CSV files.
+
+We implemented this to add our own authentication and caching logic to reduce frequent downloads of the same data.
+
+## Troubleshooting: If you see an initialization failure, verify that BQL is available and working.
+
+```
+import bql
+bq = bql.Service()
+bq.execute("get(name) for('IBM US Equity')")
+```
+
+If this fails, you are probably not running in BQuant.
+
+# AWS S3 Extension
+
+IQL provides an S3 Extension to provide an entrypoint for control of S3 data retrieval and local caching. This extension is intended to be extended to support environment-specific authentication and cache control requirments.
+
+Usage:
+
+```
+SELECT * FROM s3('s3://bucket/prefix/key/objname.parquet') as data1
+```
+
+What happens:
+
+- objname.parquet is to the iql.iqmo.DEFAULT_EXT_DIRECTORY, or the default dir if no directory is set.
+- s3(...) is replaced with a reference to the local Parquet file, allowing the database engine to read the Parquet file natively
+
+## S3 File Caching
+
+S3 files are downloaded locally and reused while the cache reference has not expired.
+
+## AWS Authentication
+
+- Default behavior: The AWS S3 extension simply calls - boto3.resource("s3"), assuming the environment is already set properly
+- Option 1: Create and store boto3 S3 resources to iql.extensions.aws_s3_extension::BOTO_S3_RESOURCES for each bucket
+
+```
+from iql.extensions import aws_s3_extension
+url_prefix = "s3://something/something"
+.... AWS CREDENTIAL STUFF ....
+s3res = boto3.resource("s3")
+aws_s3_extension.BOTO3_S3_RESOURCES[url_prefix] = s3res
+```
+
+- Option 2: Replace iql.extensions.aws_s3_extension::get_boto3_resource_for_request(), which takes a single URL parameter and returns a boto3 resource object
+
+# SKLearn Extension
+
+The SKLearn extension provides a lightweight wrapper around basic regressions, allowing regressions to be created in inline SQL statements.
+
+TODO: Complete this Section
+
+```
+df_arima = iql.execute(f"""select * from regression(data='df',
+        model='pmdarima.ARIMA', X=['{x_col}'], y=['{column}']
+        , model_order=(2,1,2), forecast=4
+        )
+        """)
+```
+
+## Model Dependencies
+
+### Arima
+
+pip install pmdarima
+
+### Prophet
+
+pip install prophet
+pip install backports.zoneinfo (?)
+
+# Caching
+
+SubQueries are often expensive and often reused while developing and refining queries. If enabled, IQL will cache the SubQuery results in memory and/or in a persistent file cache.
+
+Caching can be controlled via iql.configure:
+
+```
+def configure(
+    duration_seconds: Optional[int] = -1, cache_directory: Optional[str] = None, temp_dir: Optional[str] = None, max_processes: int = 2
+):
+```
+
+duration_seconds:
+
+```
+-1 (Default): Infinite (for life of kernel)
+None: Disabled
+int: Maximum life of the cached value from the time of creation.
+```
+
+cache_directory:
+
+```
+None (Default): Don't use a persistent file cache
+path: Location for the external file cache
+```
+
+## Caching Waterfall
+
+- nocache directive
+- cache directive
+- extension cache period
+- global \_CACHE_PERIOD
+
+## Caching Limitations
+
+Cached values are not pruned on expiration. The in memory dictionary is cleared on kernel restart. The file cache will grow unbounded until cleared:
+
+```
+from iql import q_cache # clear the in memory and file cache
+xq_cache.clear_caches()
+```
+
+## Caching Hints
+
+### cache=seconds
+
+Overrides the caching period. -1 is infinite caching.
+
+```
+iql.execute("""SELECT * FROM keyword("...", cache=60) as q1""")
+```
+
+### nocache=True
+
+Does not use any cached results
+
+```
+iql.execute("""SELECT * FROM keyword("...", nocache=True) as q1""")
+```
+
+## Caching Best Practices
+
+Caching is important to get right but depend on the data and use cache. Caching can significantly improve performance during design and development which frequently reuse unchanging data. For live data that changes frequently, an appropriate cache interval should be used to avoid reuse of stale data.
+
+If your kernels are short-lived, this is largely a non-issue, since the cache is reset automatically, unless a file cache is activated.
+
+# Database
+
+## Valid Queries
+
+In DuckDB, IQL was developed against DuckDB's statements, including SELECTs with CTE's (WITH clauses). IQL is seamless: it only modifies the extension SubQueries, and otherwise passes the results to the database.
+
+Any valid DuckDB query should be supported.
+
+When troubleshooting, check the usual suspects first:
+
+- Make sure parentheses and quotes are balanced
+  Most query errors are from forgetting a closing quote and/or parenthesis.
+- SQL uses single quotes for string literals (constants):
+
+```
+  select 'abc' # 'abc' is a string literal
+```
+
+is not the same as
+
+```
+select "abc" # "abc" is a column name
+```
+
+- Valid SQL syntax: Complex SQL queries can be cumbersome. Consider breaking a complex query into several individual steps, at least to refine the logic. This can have a negative performance impact as it defeats any database query optimization, but in practical terms, it is often beneficial.
+
+## Database Lifecycle
+
+### Default: In-Memory Database for each iql.execute()
+
+By default, a series of iql.execute() calls will create and close an in-memory DuckDB connection for each request.
+
+### Option 1: Keep Database Open
+
+Use the iql default connection setting (in-memory only), but leave the connection open:
+
+```
+con = iql.IQL.get_dbconnector().get_connection()
+try:
+  iql.execute("CREATE TABLE abc as SELECT * FROM (values(1),(2),(3))", con=con)
+  df=iql.execute("SELECT * FROM abc", con=con)
+  display(df)
+finally:
+  con.close()
+```
+
+SQL statements separated by semicolons. The entire set will be run sequentially against a single database, so side effects will be maintained.
+
+### Option 2: Create Database Externally
+
+With this method, you can use a file-based persistent database along with other connectivity options.
+
+Or, create a DuckDB Connection [duckdb.connect()](https://duckdb.org/docs/api/python/overview), such as for a file-based persistent database.
+
+```
+df=iql.execute("SELECT * FROM abc", con=con)
+```
+
+# FAQ
+
+## How can I simplify my SQL?
+
+There are several approaches to using IQL SubQueries:
+
+### Inline
+
+```
+  SELECT fields
+  FROM table1
+  JOIN table2
+    on table1.id=table2.id
+  JOIN kaggle(".....") as k3
+    on k3.dates < table2.dates
+  WHERE k3.something is true
+```
+
+### Common Table Expressions (WITH clause)
+
+CTEs are necessary when the same subquery will be transformed multiple times within a single query. CTEs are also helpful syntactic sugar: the declaration of a subquery is separate from its use, making the SELECT statement simpler.
+
+```
+  WITH k3 as (select * from kaggle(".....") WHERE something is true)
+  SELECT fields
+  FROM table1
+  JOIN table2
+    on table1.id=table2.id
+  JOIN k3
+    on k3.dates < table2.dates
+```
+
+### Storing the Data in Tables
+
+When data will be accessed by multiple queries, store the data first via CREATE TABLE / CREATE TEMP TABLE instead of running the same IQL SubQueries multiple times. IQL's caching is helpful, if enabled, but storing the data in tables provides more flexibility.
+
+```
+  CREATE [TEMP] TABLE k3 as (SELECT * FROM kaggle(".....") WHERE something is true);
+  SELECT fields
+  FROM table2
+    on table1.id=table2.id
+  JOIN k3
+    on k3.dates < table2.dates
+```
+
+## Why DuckDB as the default?
+
+We chose [DuckDB](https://duckdb.org/) as the default database module for a few reasons:
+
+- DuckDB is awesome and [fast](https://duckdb.org/2021/05/14/sql-on-pandas.html), with vectorized columnar operations.
+- It runs with no setup
+- It runs fully locally and has support for a variety of data sources
+- DuckDB's SQL language is standard
+- DuckDB natively supports Pandas
+
+## Why not a DuckDB Extensions?
+
+We didn't implement IQL as an extension for a few reasons:
+
+- Portability: DuckDB is great, but it's not the only game in town. Engines like SnowFlake are important.
+- Speed of development: Native Python is easy to develop, easy to debug, and convenient to modify and extend.
+- Performance: In our workflows, there was little performance to be gained. Runtime was dominated by external data transfer.
+
+We may still implement DuckDB extension(s) to eliminate the extra preprocess/rewrite step.
+
+## Other Databases Engines
+
+Any database can be supported by implementing a database module. IQL was written in a syntax neutral (any vendors SQL variant _should_ work) method. The key step that's dependent on the database engine is registering (or loading) the SubQuery dataframes to the database engine prior to executing the queries.
+
+Modules could be added to support other engines and formats:
+
+- [SQLDF](https://pypi.org/project/sqldf/) and [PandaSQL](https://pypi.org/project/pandasql/): Local-only databases that can connect to in-memory Pandas dataframes
+- PyArrow (w/ PySpark/Dask): SubQuery dataframes would be loaded via [pyarrow.Table.from_pandas()](https://arrow.apache.org/docs/python/pandas.html)
+- SnowFlake: During registration step, the Pandas dataframes need to be loaded via the [SnowFlake Pandas Connector](https://docs.snowflake.com/en/user-guide/python-connector-pandas)
+- Other Pandas-centric engines, such as SQLDF and PandaSQL
+
+## What about Polars?
+
+Since DuckDB supports Polars, IQL extensions could be modified to use Polars DataFrames since DuckDB supports Polars. This would be a relatively simple change, made in each extension to create a Polars DataFrame instead of a Pandas DataFrame. This could be made extensible, so the default DataFrame implementation is user selectable.
+
+## Design Principles
+
+- Extensibility: Extensions and Database Connectors can be easily modified, replaced, or extended.
+- KISS: Keep it simple. Don't add complexity.
+  - REST APIs, such as FRED: Use the complete URL, rather than building yet-another-Python-API
+  - Bloomberg BQL: Use native BQL queries without modification
+- Minimal dependencies: Extensions are loaded on-demand. Unused dependencies are not required.
+
+# Footnotes
+
+## Useful DuckDB Features
+
+### CTEs
+
+```
+import iql
+df = iql.execute("""
+  WITH c AS keyword("..."),
+      idx AS keyword("...")
+    SELECT c.*, idx.*
+    FROM c
+    JOIN idx
+      ON c.idx=idx.id""")
+display(df)
+```
+
+### Accessing Global DataFrames:
+
+```
+import iql
+import pandas as pd
+
+fun = pd.DataFrame([{'id': 'Someone', 'fun_level': 'High'}])
+iql.execute("""SELECT * FROM fun""")
+```
+
+### Copy (query) to 'file'
+
+```
+import iql
+iql.execute("""COPY (query) TO 'somefile.parquet'""")
+```
+
+## Copy to Parquet
+
+- Copy to parquet:
+  https://duckdb.org/docs/guides/import/parquet_export.html#:~:text=To%20export%20the%20data%20from,exported%20to%20a%20Parquet%20file.
+
+# Futures and Ideas
+
+## SQL ReWrite
+
+Instead of modifying the SQL in a single step, we could introduce an intermediate statement that has the same logical flow as the code today. This would make it easier to debug, allowing the user to view and debug each step.
+
+```
+SELECT * FROM fred() a JOIN fred() b on a.id=b.id
+```
+
+could be transformed first into:
+
+```
+a=fred();
+b=fred();
+SELECT * FROM a JOIN b
+```
+
+One decision needed here is how to express the first two statements: would we use a CREATE TEMP TABLE or COPY TO to store the SubQuery results, or do we introduce something like CREATE DF.
+
+## Simplifying Parsing
+
+We didn't implement a grammar, because each grammar is very platform dependent. Each database has its own product-specific grammar.
+
+The current IQL implementation first parses the SQL to extract the named functions, using the sqlparse library, then extracts the IQL subquerys by their named keywords. The SubQueries are then parsed via an AST to extract the parameters and values. Any parsing introduces risks and fragility:
+
+- It's possible that sqlparse will fail to parse certain database specific language features. We haven't encountered this yet, but it's something we're thinking about
+- It's also possible that our extraction will fail to recognize proper subqueries, due to how sqlparse extracts the tokens. The code here is not as robust as we'd like, and more testing is needed.
+
+There's a few ways to improve this:
+
+- Direct string extraction: identify subquery() blocks and extract them directly as strings, rather than parsing the entire SQL file. This would have to properly account for commenting, quoting, and nesting.
+- DuckDB (or whatever platform) extensions: use a lightweight extension to allow the database to externally call the IQL layer, rather than having IQL act as an intermediate step. Or, use a table function, which is not yet supported in SQL, only in relational API.
+
+## Caching
+
+The in-memory cache will grow unbounded within each kernel session. The expiration is only used to invalid data, but expired results are not evicted from memory if not accessed.
+
+We'll replace the in-memory cache with something more robust, probably another cache implementation such as [cachetools](https://github.com/tkem/cachetools). Alternatively, IQL could maintain a cache per "session", rather than globally.
+
+If your kernels are long-lived, clear the cache at appropriate intervals or points in your workflow:
+
+```
+iql.clear_caches()
+```
+
+## Parquet Files or PyArrow vs DataFrame
+
+In-Memory Extensions could serialize data to other formats, instead of to DataFrames.
+
+Note: This isn't required for file-based extensions like AWS S3.
+
+# Footer
+
+Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
+All Rights Reserved
```

