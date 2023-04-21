# Comparing `tmp/crunchdao-0.3.0.tar.gz` & `tmp/crunchdao-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunchdao-0.3.0.tar", max compression
+gzip compressed data, was "crunchdao-0.4.0.tar", max compression
```

## Comparing `crunchdao-0.3.0.tar` & `crunchdao-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       33 2023-03-24 18:40:10.542653 crunchdao-0.3.0/crunchdao/__init__.py
--rw-r--r--   0        0        0     8889 2023-03-24 18:40:10.542653 crunchdao-0.3.0/crunchdao/api.py
--rw-r--r--   0        0        0     1816 2023-03-24 18:40:10.542653 crunchdao-0.3.0/crunchdao/utils.py
--rw-r--r--   0        0        0      462 2023-03-24 18:40:10.542653 crunchdao-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 crunchdao-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       33 2023-04-21 18:17:18.532231 crunchdao-0.4.0/crunchdao/__init__.py
+-rwxr-xr-x   0        0        0    12829 2023-04-21 18:17:18.532231 crunchdao-0.4.0/crunchdao/api.py
+-rwxr-xr-x   0        0        0     2118 2023-04-21 18:17:18.532231 crunchdao-0.4.0/crunchdao/utils.py
+-rwxr-xr-x   0        0        0      481 2023-04-21 18:17:18.532231 crunchdao-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 crunchdao-0.4.0/PKG-INFO
```

### Comparing `crunchdao-0.3.0/crunchdao/utils.py` & `crunchdao-0.4.0/crunchdao/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import logging
 
 import tqdm
 import requests
-
+import pandas as pd
+import holidays
 
 logger = logging.getLogger(__name__)
 
 
 def download_file(url: str, dest_path: str,
                   show_progress_bars: bool = True) -> str:
     """downloads a file and shows a progress bar. allows resuming a download"""
@@ -46,7 +47,14 @@
     # Update progress bar to reflect how much of the file is already downloaded
     pbar.update(file_size)
     with open(dest_path, "ab") as dest_file:
         for chunk in req.iter_content(1024):
             dest_file.write(chunk)
             pbar.update(1024)
     return dest_path
+
+def is_trading_day(date: pd.Timestamp) -> bool:
+    """Tells if a given date is a trading day"""
+    us_holidays = holidays.NYSE()
+    is_bday = bool(len(pd.bdate_range(date, date)))
+    is_not_holiday = date not in us_holidays
+    return is_bday and is_not_holiday
```

