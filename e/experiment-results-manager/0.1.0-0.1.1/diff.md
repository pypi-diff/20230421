# Comparing `tmp/experiment-results-manager-0.1.0.tar.gz` & `tmp/experiment-results-manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-results-manager-0.1.0.tar", max compression
+gzip compressed data, was "experiment-results-manager-0.1.1.tar", max compression
```

## Comparing `experiment-results-manager-0.1.0.tar` & `experiment-results-manager-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      446 2023-04-18 23:12:08.840015 experiment-results-manager-0.1.0/experiment_results_manager/__init__.py
--rw-r--r--   0        0        0      797 2023-04-18 18:29:37.900015 experiment-results-manager-0.1.0/experiment_results_manager/artifact.py
--rw-r--r--   0        0        0     3576 2023-04-19 09:05:46.502943 experiment-results-manager-0.1.0/experiment_results_manager/compare_runs.py
--rw-r--r--   0        0        0     7576 2023-04-19 19:44:00.476585 experiment-results-manager-0.1.0/experiment_results_manager/experiment_run.py
--rw-r--r--   0        0        0     1600 2023-04-19 09:09:15.023327 experiment-results-manager-0.1.0/experiment_results_manager/html_util.py
--rw-r--r--   0        0        0     3615 2023-04-18 23:45:16.069628 experiment-results-manager-0.1.0/experiment_results_manager/serde.py
--rw-r--r--   0        0        0      946 2023-04-20 06:33:17.854789 experiment-results-manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      630 2023-04-20 06:34:08.438074 experiment-results-manager-0.1.0/setup.py
--rw-r--r--   0        0        0      425 2023-04-20 06:34:08.438223 experiment-results-manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1230 2023-04-20 06:37:34.398517 experiment-results-manager-0.1.1/README.md
+-rw-r--r--   0        0        0      446 2023-04-18 23:12:08.840015 experiment-results-manager-0.1.1/experiment_results_manager/__init__.py
+-rw-r--r--   0        0        0      797 2023-04-18 18:29:37.900015 experiment-results-manager-0.1.1/experiment_results_manager/artifact.py
+-rw-r--r--   0        0        0     4518 2023-04-21 13:57:29.047715 experiment-results-manager-0.1.1/experiment_results_manager/compare_runs.py
+-rw-r--r--   0        0        0     7677 2023-04-20 18:52:12.869094 experiment-results-manager-0.1.1/experiment_results_manager/experiment_run.py
+-rw-r--r--   0        0        0     2051 2023-04-21 11:34:09.217133 experiment-results-manager-0.1.1/experiment_results_manager/html_util.py
+-rw-r--r--   0        0        0     3615 2023-04-18 23:45:16.069628 experiment-results-manager-0.1.1/experiment_results_manager/serde.py
+-rw-r--r--   0        0        0     1161 2023-04-21 16:04:48.185974 experiment-results-manager-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1992 2023-04-21 16:05:04.075236 experiment-results-manager-0.1.1/setup.py
+-rw-r--r--   0        0        0     1973 2023-04-21 16:05:04.075391 experiment-results-manager-0.1.1/PKG-INFO
```

### Comparing `experiment-results-manager-0.1.0/experiment_results_manager/artifact.py` & `experiment-results-manager-0.1.1/experiment_results_manager/artifact.py`

 * *Files identical despite different names*

### Comparing `experiment-results-manager-0.1.0/experiment_results_manager/experiment_run.py` & `experiment-results-manager-0.1.1/experiment_results_manager/experiment_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from datetime import datetime
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import matplotlib.axes
 import matplotlib.figure
 import plotly
 
 from experiment_results_manager.artifact import Artifact, ArtifactType
 from experiment_results_manager.html_util import matplotlib_fig_to_bytes
@@ -52,44 +52,45 @@
 
     def __init__(
         self,
         experiment_id: str,
         variant_id: str = "main",
         run_id: Optional[str] = None,
         timestamp_utc: Optional[datetime] = None,
+        features: Optional[List[str]] = None,
         params: Optional[Dict[str, Union[str, int, float]]] = None,
         metrics: Optional[Dict[str, Union[str, int, float]]] = None,
         dicts: Optional[Dict[str, Dict[str, Any]]] = None,
         artifacts: Optional[Dict[str, Artifact]] = None,
     ) -> None:
         """
         Initializes a new `ExperimentRun` object with the given experiment_id,
         `variant_id`, `run_id`, and `timestamp_utc`. If `timestamp_utc` is not provided,
         it defaults to the current UTC datetime. If `run_id` is not provided, it
         is generated from the `timestamp_utc` using the format "%Y_%m_%d__%H_%M_%S".
         """
 
-        if timestamp_utc is None:
-            self.timestamp_utc = datetime.utcnow()
-        else:
-            self.timestamp_utc = timestamp_utc
-
+        self.experiment_id = experiment_id
+        self.variant_id = variant_id
+        self.timestamp_utc = (
+            timestamp_utc if timestamp_utc is not None else datetime.utcnow()
+        )
         if run_id is None:
             self.run_id = self.timestamp_utc.strftime("%Y_%m_%d__%H_%M_%S")
         else:
             self.run_id = run_id
 
-        self.variant_id = variant_id
-        self.experiment_id = experiment_id
+        self.features: List[str] = features if features is not None else []
         self.params: Dict[str, Union[str, int, float]] = (
             params if params is not None else {}
         )
         self.metrics: Dict[str, Union[str, int, float]] = (
             metrics if metrics is not None else {}
         )
+
         self.dicts: Dict[str, Dict[str, Any]] = dicts if dicts is not None else {}
         self.artifacts: Dict[str, Artifact] = artifacts if artifacts is not None else {}
 
     def log_param(self, key: str, value: Union[str, int, float]) -> None:
         """Logs a parameter to the experiment run."""
         self.params[key] = value
```

### Comparing `experiment-results-manager-0.1.0/experiment_results_manager/serde.py` & `experiment-results-manager-0.1.1/experiment_results_manager/serde.py`

 * *Files identical despite different names*

### Comparing `experiment-results-manager-0.1.0/pyproject.toml` & `experiment-results-manager-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [tool.poetry]
 name = "experiment-results-manager"
-version = "0.1.0"
-description = ""
-authors = ["Your Name <you@example.com>"]
+version = "0.1.1"
+description = "Light-weight experiment tracker"
+authors = ["sa- <name@example.com>"]
+repository = "https://github.com/ml-cyclops/experiment-results-manager"
+documentation = "https://github.com/ml-cyclops/experiment-results-manager/blob/main/README.md"
+readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8"
 fsspec = ">=2021.4"
 pydantic = "^1.6"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.2.2"
 black = "^23.3.0"
 ruff = "^0.0.261"
```

