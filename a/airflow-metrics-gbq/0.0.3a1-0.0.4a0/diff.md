# Comparing `tmp/airflow_metrics_gbq-0.0.3a1.tar.gz` & `tmp/airflow_metrics_gbq-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_metrics_gbq-0.0.3a1.tar", max compression
+gzip compressed data, was "airflow_metrics_gbq-0.0.4a0.tar", max compression
```

## Comparing `airflow_metrics_gbq-0.0.3a1.tar` & `airflow_metrics_gbq-0.0.4a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1296 2023-04-19 21:27:07.759137 airflow_metrics_gbq-0.0.3a1/LICENSE
--rw-r--r--   0        0        0      397 2023-04-19 21:27:07.759137 airflow_metrics_gbq-0.0.3a1/README.md
--rw-r--r--   0        0        0        0 2023-04-19 21:27:07.759137 airflow_metrics_gbq-0.0.3a1/airflow_metrics_gbq/__init__.py
--rw-r--r--   0        0        0     7591 2023-04-19 21:27:07.759137 airflow_metrics_gbq-0.0.3a1/airflow_metrics_gbq/metrics.py
--rw-r--r--   0        0        0      700 2023-04-19 21:27:07.759137 airflow_metrics_gbq-0.0.3a1/airflow_metrics_gbq/utils/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-19 21:27:07.759137 airflow_metrics_gbq-0.0.3a1/airflow_metrics_gbq/utils/gbq_connector.py
--rw-r--r--   0        0        0     1266 2023-04-19 21:27:07.759137 airflow_metrics_gbq-0.0.3a1/pyproject.toml
--rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.3a1/PKG-INFO
+-rw-r--r--   0        0        0     1296 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/LICENSE
+-rw-r--r--   0        0        0     2549 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/__init__.py
+-rw-r--r--   0        0        0     7541 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/metrics.py
+-rw-r--r--   0        0        0      700 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/utils/__init__.py
+-rw-r--r--   0        0        0     1674 2023-04-20 22:07:21.054985 airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/utils/gbq_connector.py
+-rw-r--r--   0        0        0     1300 2023-04-20 22:07:21.058985 airflow_metrics_gbq-0.0.4a0/pyproject.toml
+-rw-r--r--   0        0        0     3737 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.4a0/PKG-INFO
```

### Comparing `airflow_metrics_gbq-0.0.3a1/LICENSE` & `airflow_metrics_gbq-0.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.3a1/airflow_metrics_gbq/metrics.py` & `airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 import os
 import socket
 import time
 import random
 from typing import Optional
+from enum import Enum, unique
 from collections import defaultdict
+from dataclasses import dataclass
 import pandas as pd
 
 from airflow_metrics_gbq.utils import GoogleBigQueryConnector, setup_gcloud_logging
 
 
 # pylint: disable=too-few-public-methods
+@dataclass
 class Point:
     """Represents a single metric record"""
 
-    def __init__(
-        self,
-        app,
-        domain,
-        value,
-        timestamp,
-        check: Optional[str] = None,
-        name: Optional[str] = None,
-    ):
-        self.app = app
-        self.domain = domain
-        self.check = check
-        self.value = value
-        self.timestamp = timestamp
-        self.name = name
+    app: str
+    domain: str
+    value: float
+    timestamp: float
+    check: Optional[str] = None
+    name: Optional[str] = None
 
 
-class Measure:
+@unique
+class Measure(Enum):
     """Type of measure"""
 
     COUNT = "count"
     LAST = "last"
     TIMER = "timer"
 
-
-def from_mtype(mtype) -> Measure:
-    """Maps a suffix to a measure type"""
-
-    mtype_map = {
-        "c": Measure.COUNT,
-        "g": Measure.LAST,
-        "ms": Measure.TIMER,
-        "s": Measure.TIMER,
-    }
-    return mtype_map[mtype]
+    @classmethod
+    def from_mtype(cls, mtype: str) -> "Measure":
+        """Maps a suffix to a measure type"""
+
+        mtype_map = {
+            "c": Measure.COUNT,
+            "g": Measure.LAST,
+            "ms": Measure.TIMER,
+            "s": Measure.TIMER,
+        }
+        return mtype_map[mtype]
 
 
 class PointWithType:
     """A single metric record along with the Measure type"""
 
     SEPARATOR = "|"
 
@@ -59,15 +54,15 @@
         self.point = point
         self.measure = measure
 
     @staticmethod
     def from_record(record: str) -> "PointWithType":
         """Creates an instance from a raw record"""
         line, mtype = record.split(PointWithType.SEPARATOR)
-        mtype = from_mtype(mtype)
+        mtype = Measure.from_mtype(mtype)
         line, val = line.split(":")
         fields = line.split(".")
         timestamp = time.time()
         if len(fields) == 4:
             point = Point(fields[0], fields[1], float(val), timestamp, fields[2], fields[3])
         elif len(fields) == 3:
             point = Point(fields[0], fields[1], float(val), timestamp, fields[2])
```

### Comparing `airflow_metrics_gbq-0.0.3a1/airflow_metrics_gbq/utils/__init__.py` & `airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.3a1/airflow_metrics_gbq/utils/gbq_connector.py` & `airflow_metrics_gbq-0.0.4a0/airflow_metrics_gbq/utils/gbq_connector.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.3a1/pyproject.toml` & `airflow_metrics_gbq-0.0.4a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-metrics-gbq"
-version = "0.0.3a1"
+version = "0.0.4a0"
 description = "Airflow metrics to Google BigQuery"
 authors = ["Shaurya Rawat <rawatshaurya1994@gmail.com>"]
 license = "BSD2"
 readme = "README.md"
 homepage="https://github.com/abyssnlp/airflow-metrics-gbq"
 repository="https://github.com/abyssnlp/airflow-metrics-gbq"
 include=[
@@ -20,15 +20,15 @@
     "License :: OSI Approved :: BSD License"
 ]
 packages = [{include = "airflow_metrics_gbq"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pandas = "^2.0.0"
-google-cloud-bigquery = "^3.9.0"
+google-cloud-bigquery = {extras = ["pandas"], version = "^3.10.0"}
 google-api-python-client = "^2.85.0"
 google-cloud-logging = "^3.5.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["d"], version = "^23.3.0"}
 pylint = "^2.17.2"
```

