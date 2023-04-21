# Comparing `tmp/chronus-0.2.1.tar.gz` & `tmp/chronus-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chronus-0.2.1.tar", max compression
+gzip compressed data, was "chronus-0.2.2.tar", max compression
```

## Comparing `chronus-0.2.1.tar` & `chronus-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-02-28 09:33:02.453690 chronus-0.2.1/LICENSE
--rw-r--r--   0        0        0    10481 2023-04-17 11:01:17.462307 chronus-0.2.1/README.md
--rw-r--r--   0        0        0     1121 2023-04-17 10:32:37.217149 chronus-0.2.1/chronus/SystemIntegration/FileRepository.py
--rw-r--r--   0        0        0        1 2023-04-17 10:44:37.558827 chronus-0.2.1/chronus/SystemIntegration/__init__.py
--rw-r--r--   0        0        0     1550 2023-04-17 10:44:37.560286 chronus-0.2.1/chronus/SystemIntegration/hpcg.py
--rw-r--r--   0        0        0      195 2023-04-17 10:32:37.219423 chronus-0.2.1/chronus/SystemIntegration/repository.py
--rw-r--r--   0        0        0      330 2023-04-17 10:14:26.979910 chronus-0.2.1/chronus/__init__.py
--rw-r--r--   0        0        0     3724 2023-04-17 10:44:37.585076 chronus-0.2.1/chronus/__main__.py
--rw-r--r--   0        0        0        0 2023-04-17 10:14:26.980936 chronus-0.2.1/chronus/domain/__init__.py
--rw-r--r--   0        0        0      313 2023-02-28 09:33:02.456874 chronus-0.2.1/chronus/example.py
--rw-r--r--   0        0        0      409 2023-04-17 10:32:37.221715 chronus-0.2.1/chronus/model/Run.py
--rw-r--r--   0        0        0        0 2023-04-17 10:32:37.222095 chronus-0.2.1/chronus/model/__init__.py
--rw-r--r--   0        0        0     2091 2023-04-17 10:32:37.223079 chronus-0.2.1/chronus/model/svm.py
--rw-r--r--   0        0        0     1496 2023-04-17 10:44:37.562774 chronus-0.2.1/chronus/vis/__init__.py
--rw-r--r--   0        0        0     3583 2023-04-17 11:01:34.731519 chronus-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    11620 1970-01-01 00:00:00.000000 chronus-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-28 09:33:02.453690 chronus-0.2.2/LICENSE
+-rw-r--r--   0        0        0    10481 2023-04-17 11:01:17.462307 chronus-0.2.2/README.md
+-rw-r--r--   0        0        0     1122 2023-04-21 06:57:23.169699 chronus-0.2.2/chronus/SystemIntegration/FileRepository.py
+-rw-r--r--   0        0        0        1 2023-04-17 10:44:37.558827 chronus-0.2.2/chronus/SystemIntegration/__init__.py
+-rw-r--r--   0        0        0     1977 2023-04-21 13:37:43.020958 chronus-0.2.2/chronus/SystemIntegration/cpu_info_service.py
+-rw-r--r--   0        0        0     1551 2023-04-21 06:57:23.179206 chronus-0.2.2/chronus/SystemIntegration/hpcg.py
+-rw-r--r--   0        0        0      200 2023-04-21 11:06:34.779261 chronus-0.2.2/chronus/SystemIntegration/repository.py
+-rw-r--r--   0        0        0      330 2023-04-17 10:14:26.979910 chronus-0.2.2/chronus/__init__.py
+-rw-r--r--   0        0        0     4044 2023-04-21 13:37:40.245593 chronus-0.2.2/chronus/__main__.py
+-rw-r--r--   0        0        0     1497 2023-04-21 06:57:23.157333 chronus-0.2.2/chronus/cli/__init__.py
+-rw-r--r--   0        0        0     1224 2023-04-21 13:37:43.015999 chronus-0.2.2/chronus/domain/Run.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:14:26.980936 chronus-0.2.2/chronus/domain/__init__.py
+-rw-r--r--   0        0        0     2075 2023-04-21 13:37:43.018032 chronus-0.2.2/chronus/domain/benchmark_service.py
+-rw-r--r--   0        0        0      975 2023-04-21 13:37:40.293638 chronus-0.2.2/chronus/domain/configuration.py
+-rw-r--r--   0        0        0        0 2023-04-21 06:56:28.522159 chronus-0.2.2/chronus/domain/interfaces/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-21 06:53:32.150630 chronus-0.2.2/chronus/domain/interfaces/application_runner_interface.py
+-rw-r--r--   0        0        0       91 2023-04-21 06:54:31.741981 chronus-0.2.2/chronus/domain/interfaces/benchmark_run_repository_interface.py
+-rw-r--r--   0        0        0      300 2023-04-21 13:37:42.986739 chronus-0.2.2/chronus/domain/interfaces/cpu_info_service_interface.py
+-rw-r--r--   0        0        0      137 2023-04-21 06:56:09.236466 chronus-0.2.2/chronus/domain/interfaces/system_service_interface.py
+-rw-r--r--   0        0        0      146 2023-04-21 06:38:37.130694 chronus-0.2.2/chronus/domain/system_sample.py
+-rw-r--r--   0        0        0      313 2023-02-28 09:33:02.456874 chronus-0.2.2/chronus/example.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:32:37.222095 chronus-0.2.2/chronus/model/__init__.py
+-rw-r--r--   0        0        0     2092 2023-04-21 06:57:22.994327 chronus-0.2.2/chronus/model/svm.py
+-rw-r--r--   0        0        0     3611 2023-04-21 13:41:43.715379 chronus-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    11620 1970-01-01 00:00:00.000000 chronus-0.2.2/PKG-INFO
```

### Comparing `chronus-0.2.1/LICENSE` & `chronus-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chronus-0.2.1/README.md` & `chronus-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `chronus-0.2.1/chronus/SystemIntegration/FileRepository.py` & `chronus-0.2.2/chronus/SystemIntegration/FileRepository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import IO, Callable
 
 import io
 from pprint import pprint
 
-from chronus.model.Run import Run
+from chronus.domain.Run import Run
 from chronus.SystemIntegration.repository import Repository
 
 
 class FileRepository(Repository):
     _path: str
 
     def _file_factory(self, path, mode):
```

### Comparing `chronus-0.2.1/chronus/SystemIntegration/hpcg.py` & `chronus-0.2.2/chronus/SystemIntegration/hpcg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import re
 from pprint import pprint
 
-from chronus.model.Run import Run
+from chronus.domain.Run import Run
 
 
 class HpcgService:
     _output: str
 
     def __init__(self, runner=None):
         self._runner = runner or HpcgRunner()
```

### Comparing `chronus-0.2.1/chronus/__main__.py` & `chronus-0.2.2/chronus/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 
 import typer
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.pretty import pprint
 
 from chronus import version
+from chronus.cli import fake_data, plot_energy
 from chronus.model.svm import config_model
+from chronus.SystemIntegration.cpu_info_service import LsCpuInfoService
 from chronus.SystemIntegration.FileRepository import FileRepository
 from chronus.SystemIntegration.hpcg import HpcgService
 from chronus.SystemIntegration.repository import Repository
-from chronus.vis import plot_energy, fake_data
 
 name_as_grad = "^[[38;2;244;59;71mc^[[39m^[[38;2;215;59;84mh^[[39m^[[38;2;186;59;97mr^[[39m^[[38;2;157;59;110mo^[[39m^[[38;2;127;58;122mn^[[39m^[[38;2;98;58;135mu^[[39m^[[38;2;69;58;148ms^[[39m"
 name = "chronus"
 
 
 class Color(str, Enum):
     white = "white"
@@ -134,19 +135,28 @@
 def solver():
     data = fake_data()
 
     best_config = config_model(data)
 
     pprint(best_config)
 
-@app.command(name="slurm-config-json")
-def get_config(cpu: str = typer.Argument(..., help="The cpu model to get the config for")):
 
+@app.command(name="slurm-config")
+def get_config(cpu: str = typer.Argument(..., help="The cpu model to get the config for")):
     config = {
         "cores": 2,
         "frequency": 2_200_000,
     }
 
     print(json.dumps(config))
 
+
+@app.command(name="cpu")
+def debug():
+    cpu_service = LsCpuInfoService()
+    pprint(f"CPU:         {cpu_service.get_cpu_info().cpu}")
+    pprint(f"Frequencies: {cpu_service.get_frequencies()}")
+    pprint(f"Cores:       {cpu_service.get_cores()}")
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `chronus-0.2.1/chronus/model/svm.py` & `chronus-0.2.2/chronus/model/svm.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from pprint import pprint
 
 from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import GridSearchCV, train_test_split
 from sklearn.svm import SVR
 
-from chronus.model.Run import Run
+from chronus.domain.Run import Run
 
 param_grid = {
     "C": [0.1, 1, 10],
     "kernel": ["linear", "poly", "rbf", "sigmoid"],
     "gamma": ["scale", "auto"],
 }
```

### Comparing `chronus-0.2.1/chronus/vis/__init__.py` & `chronus-0.2.2/chronus/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from random import choice, randrange, uniform
 
 import matplotlib.pyplot as plt
 import numpy as np
 from mpl_toolkits.mplot3d import Axes3D
 
-from chronus.model.Run import Run
+from chronus.domain.Run import Run
 
 
 def fake_data() -> list[Run]:
     # check if data set is cached in file
     file_path = "/home/anders/projects/chronus/out/chronus_fake_run.json"
     if os.path.isfile(file_path):
         data = json.load(open(file_path))
```

### Comparing `chronus-0.2.1/pyproject.toml` & `chronus-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "chronus"
-version = "0.2.1"
+version = "0.2.2"
 description = "A energy scheduling model, build for HPC."
 readme = "README.md"
 authors = ["chronus <aaspringborg@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/AndersSpringborg/chronus"
 homepage = "https://github.com/AndersSpringborg/chronus"
 
@@ -53,14 +53,15 @@
 pyupgrade = "^3.3.1"
 safety = "^2.3.5"
 coverage = "^7.2.3"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.2.0"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.9.1"
+pytest-freezegun = "^0.4.2"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py39"]
 line-length = 100
 color = true
```

### Comparing `chronus-0.2.1/PKG-INFO` & `chronus-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chronus
-Version: 0.2.1
+Version: 0.2.2
 Summary: A energy scheduling model, build for HPC.
 Home-page: https://github.com/AndersSpringborg/chronus
 License: MIT
 Author: chronus
 Author-email: aaspringborg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

