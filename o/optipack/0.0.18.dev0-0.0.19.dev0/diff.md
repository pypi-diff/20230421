# Comparing `tmp/optipack-0.0.18.dev0.tar.gz` & `tmp/optipack-0.0.19.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optipack-0.0.18.dev0.tar", max compression
+gzip compressed data, was "optipack-0.0.19.dev0.tar", max compression
```

## Comparing `optipack-0.0.18.dev0.tar` & `optipack-0.0.19.dev0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1072 2023-02-02 02:52:49.676807 optipack-0.0.18.dev0/LICENSE
--rw-r--r--   0        0        0      795 2023-02-22 03:50:53.157490 optipack-0.0.18.dev0/README.md
--rw-r--r--   0        0        0     8196 2023-02-09 02:34:16.755095 optipack-0.0.18.dev0/optipack/.DS_Store
--rw-r--r--   0        0        0      393 2023-02-23 04:45:57.676772 optipack-0.0.18.dev0/optipack/.config/app_start.yaml
--rw-r--r--   0        0        0     1152 2023-03-28 07:59:00.285290 optipack-0.0.18.dev0/optipack/.config/connection_config.yaml
--rw-r--r--   0        0        0     1105 2023-02-10 10:14:39.318351 optipack-0.0.18.dev0/optipack/.config/hyperparam_config.yaml
--rw-r--r--   0        0        0      182 2023-02-15 09:40:56.333654 optipack-0.0.18.dev0/optipack/.config/project_structure.yaml
--rw-r--r--   0        0        0      193 2023-02-10 10:47:35.669118 optipack-0.0.18.dev0/optipack/.config/run_config.yaml
--rw-r--r--   0        0        0      174 2023-04-11 04:35:43.491296 optipack-0.0.18.dev0/optipack/__init__.py
--rw-r--r--   0        0        0      487 2023-04-11 04:17:56.303032 optipack-0.0.18.dev0/optipack/__main__.py
--rw-r--r--   0        0        0     6148 2023-02-08 11:02:11.605877 optipack-0.0.18.dev0/optipack/asset/.DS_Store
--rw-r--r--   0        0        0    64098 2023-02-09 02:35:39.601968 optipack-0.0.18.dev0/optipack/asset/logo-large.png
--rw-r--r--   0        0        0    14305 2023-02-09 02:35:39.602667 optipack-0.0.18.dev0/optipack/asset/logo-small.png
--rw-r--r--   0        0        0      473 2023-02-10 10:23:56.503936 optipack-0.0.18.dev0/optipack/asset/message.txt
--rw-r--r--   0        0        0       98 2023-02-10 12:04:37.999291 optipack-0.0.18.dev0/optipack/asset/tree_vis.yaml
--rw-r--r--   0        0        0     1216 2023-03-20 02:22:23.786659 optipack-0.0.18.dev0/optipack/cli.py
--rw-r--r--   0        0        0      145 2023-04-04 08:13:01.558291 optipack-0.0.18.dev0/optipack/core/automl/builder/__init__.py
--rw-r--r--   0        0        0     3380 2023-04-05 08:46:46.918861 optipack-0.0.18.dev0/optipack/core/automl/builder/base.py
--rw-r--r--   0        0        0     2930 2023-04-05 11:24:39.834311 optipack-0.0.18.dev0/optipack/core/automl/builder/data_builder.py
--rw-r--r--   0        0        0     1219 2023-04-05 11:16:43.812793 optipack-0.0.18.dev0/optipack/core/automl/builder/metric_builder.py
--rw-r--r--   0        0        0     2067 2023-04-05 10:40:24.284172 optipack-0.0.18.dev0/optipack/core/automl/builder/model_builder.py
--rw-r--r--   0        0        0       24 2023-04-04 02:51:40.046071 optipack-0.0.18.dev0/optipack/core/automl/runner/__init__.py
--rw-r--r--   0        0        0      984 2023-04-06 08:45:17.640576 optipack-0.0.18.dev0/optipack/core/automl/runner/base.py
--rw-r--r--   0        0        0        0 2023-04-04 02:51:40.046557 optipack-0.0.18.dev0/optipack/core/automl/runner/evaluator_runner.py
--rw-r--r--   0        0        0        0 2023-04-04 02:51:40.046843 optipack-0.0.18.dev0/optipack/core/automl/runner/runner_config.py
--rw-r--r--   0        0        0      181 2023-04-06 08:45:17.641026 optipack-0.0.18.dev0/optipack/core/automl/runner/trainer_runner.py
--rw-r--r--   0        0        0     1012 2023-04-07 10:48:16.828004 optipack-0.0.18.dev0/optipack/core/fileio/reader_misc.py
--rw-r--r--   0        0        0     8364 2023-04-14 11:26:26.044156 optipack-0.0.18.dev0/optipack/core/fileio/storage_io.py
--rw-r--r--   0        0        0      741 2023-04-07 08:35:16.155017 optipack-0.0.18.dev0/optipack/core/fileio/writer_misc.py
--rw-r--r--   0        0        0      120 2023-04-04 03:01:01.201396 optipack-0.0.18.dev0/optipack/core/logger/__init__.py
--rw-r--r--   0        0        0      746 2023-04-11 04:01:15.541303 optipack-0.0.18.dev0/optipack/core/logger/base.py
--rw-r--r--   0        0        0      396 2023-03-29 11:10:16.995306 optipack-0.0.18.dev0/optipack/core/logger/logger.cfg
--rw-r--r--   0        0        0     1678 2023-04-11 03:49:00.169702 optipack-0.0.18.dev0/optipack/core/logger/otp_logger.py
--rw-r--r--   0        0        0      977 2023-04-04 02:51:40.048824 optipack-0.0.18.dev0/optipack/core/manager/automl_manager.py
--rw-r--r--   0        0        0     3727 2023-04-06 08:45:17.642258 optipack-0.0.18.dev0/optipack/core/manager/automodel_manager.py
--rw-r--r--   0        0        0      574 2023-04-04 02:51:40.050343 optipack-0.0.18.dev0/optipack/core/manager/run_manager.py
--rw-r--r--   0        0        0     2251 2023-03-20 10:11:52.420417 optipack-0.0.18.dev0/optipack/core/typing.py
--rw-r--r--   0        0        0      119 2023-04-04 03:01:16.002447 optipack-0.0.18.dev0/optipack/core/visualizer/__init__.py
--rw-r--r--   0        0        0      250 2023-03-30 10:37:47.836408 optipack-0.0.18.dev0/optipack/core/visualizer/base.py
--rw-r--r--   0        0        0     4210 2023-04-03 10:37:54.018736 optipack-0.0.18.dev0/optipack/core/visualizer/otp_visualizer.py
--rw-r--r--   0        0        0     1033 2023-04-11 04:57:10.176206 optipack-0.0.18.dev0/optipack/internal_utils/file_util.py
--rw-r--r--   0        0        0     3775 2023-03-21 10:03:49.090579 optipack-0.0.18.dev0/optipack/internal_utils/terminal_util.py
--rw-r--r--   0        0        0      155 2023-04-10 10:17:01.113759 optipack-0.0.18.dev0/optipack/sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 05:14:38.498269 optipack-0.0.18.dev0/optipack/sdk/optipack_env_controller.py
--rw-r--r--   0        0        0     1038 2023-02-11 02:42:42.365644 optipack-0.0.18.dev0/optipack/sdk/optipack_init.py
--rw-r--r--   0        0        0     4016 2023-04-11 08:41:19.143635 optipack-0.0.18.dev0/optipack/sdk/optipack_logger.py
--rw-r--r--   0        0        0     6046 2023-03-21 10:05:25.153804 optipack-0.0.18.dev0/optipack/sdk/optipack_project_generator.py
--rw-r--r--   0        0        0      158 2023-02-23 08:07:04.463928 optipack-0.0.18.dev0/optipack/sdk/optipack_run.py
--rw-r--r--   0        0        0      235 2023-04-11 04:17:27.043905 optipack-0.0.18.dev0/optipack/sdk/optipack_utils.py
--rw-r--r--   0        0        0      579 2023-04-14 17:40:45.789556 optipack-0.0.18.dev0/pyproject.toml
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 optipack-0.0.18.dev0/setup.py
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 optipack-0.0.18.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-02 02:52:49.676807 optipack-0.0.19.dev0/LICENSE
+-rw-r--r--   0        0        0      795 2023-02-22 03:50:53.157490 optipack-0.0.19.dev0/README.md
+-rw-r--r--   0        0        0     8196 2023-02-09 02:34:16.755095 optipack-0.0.19.dev0/optipack/.DS_Store
+-rw-r--r--   0        0        0      393 2023-02-23 04:45:57.676772 optipack-0.0.19.dev0/optipack/.config/app_start.yaml
+-rw-r--r--   0        0        0     1152 2023-03-28 07:59:00.285290 optipack-0.0.19.dev0/optipack/.config/connection_config.yaml
+-rw-r--r--   0        0        0     1105 2023-02-10 10:14:39.318351 optipack-0.0.19.dev0/optipack/.config/hyperparam_config.yaml
+-rw-r--r--   0        0        0      182 2023-02-15 09:40:56.333654 optipack-0.0.19.dev0/optipack/.config/project_structure.yaml
+-rw-r--r--   0        0        0      193 2023-02-10 10:47:35.669118 optipack-0.0.19.dev0/optipack/.config/run_config.yaml
+-rw-r--r--   0        0        0      174 2023-04-11 04:35:43.491296 optipack-0.0.19.dev0/optipack/__init__.py
+-rw-r--r--   0        0        0      487 2023-04-11 04:17:56.303032 optipack-0.0.19.dev0/optipack/__main__.py
+-rw-r--r--   0        0        0     6148 2023-02-08 11:02:11.605877 optipack-0.0.19.dev0/optipack/asset/.DS_Store
+-rw-r--r--   0        0        0    64098 2023-02-09 02:35:39.601968 optipack-0.0.19.dev0/optipack/asset/logo-large.png
+-rw-r--r--   0        0        0    14305 2023-02-09 02:35:39.602667 optipack-0.0.19.dev0/optipack/asset/logo-small.png
+-rw-r--r--   0        0        0      473 2023-02-10 10:23:56.503936 optipack-0.0.19.dev0/optipack/asset/message.txt
+-rw-r--r--   0        0        0       98 2023-02-10 12:04:37.999291 optipack-0.0.19.dev0/optipack/asset/tree_vis.yaml
+-rw-r--r--   0        0        0     1216 2023-03-20 02:22:23.786659 optipack-0.0.19.dev0/optipack/cli.py
+-rw-r--r--   0        0        0      257 2023-04-19 04:49:17.885432 optipack-0.0.19.dev0/optipack/core/automl/builder/__init__.py
+-rw-r--r--   0        0        0     3380 2023-04-05 08:46:46.918861 optipack-0.0.19.dev0/optipack/core/automl/builder/base.py
+-rw-r--r--   0        0        0     2963 2023-04-19 04:50:11.565658 optipack-0.0.19.dev0/optipack/core/automl/builder/data_builder.py
+-rw-r--r--   0        0        0     1252 2023-04-19 04:50:50.124725 optipack-0.0.19.dev0/optipack/core/automl/builder/metric_builder.py
+-rw-r--r--   0        0        0     2100 2023-04-19 04:51:13.529341 optipack-0.0.19.dev0/optipack/core/automl/builder/model_builder.py
+-rw-r--r--   0        0        0       51 2023-04-19 04:52:13.961098 optipack-0.0.19.dev0/optipack/core/automl/runner/__init__.py
+-rw-r--r--   0        0        0      984 2023-04-06 08:45:17.640576 optipack-0.0.19.dev0/optipack/core/automl/runner/base.py
+-rw-r--r--   0        0        0        0 2023-04-04 02:51:40.046557 optipack-0.0.19.dev0/optipack/core/automl/runner/evaluator_runner.py
+-rw-r--r--   0        0        0        0 2023-04-04 02:51:40.046843 optipack-0.0.19.dev0/optipack/core/automl/runner/runner_config.py
+-rw-r--r--   0        0        0      181 2023-04-06 08:45:17.641026 optipack-0.0.19.dev0/optipack/core/automl/runner/trainer_runner.py
+-rw-r--r--   0        0        0     1012 2023-04-07 10:48:16.828004 optipack-0.0.19.dev0/optipack/core/fileio/reader_misc.py
+-rw-r--r--   0        0        0     8407 2023-04-21 08:52:22.061222 optipack-0.0.19.dev0/optipack/core/fileio/storage_io.py
+-rw-r--r--   0        0        0      741 2023-04-07 08:35:16.155017 optipack-0.0.19.dev0/optipack/core/fileio/writer_misc.py
+-rw-r--r--   0        0        0      140 2023-04-19 04:41:50.728393 optipack-0.0.19.dev0/optipack/core/logger/__init__.py
+-rw-r--r--   0        0        0      746 2023-04-11 04:01:15.541303 optipack-0.0.19.dev0/optipack/core/logger/base.py
+-rw-r--r--   0        0        0      396 2023-03-29 11:10:16.995306 optipack-0.0.19.dev0/optipack/core/logger/logger.cfg
+-rw-r--r--   0        0        0     1893 2023-04-20 10:49:19.728342 optipack-0.0.19.dev0/optipack/core/logger/otp_logger.py
+-rw-r--r--   0        0        0     1076 2023-04-19 08:02:11.226814 optipack-0.0.19.dev0/optipack/core/manager/automl_manager.py
+-rw-r--r--   0        0        0     3745 2023-04-19 08:02:42.526653 optipack-0.0.19.dev0/optipack/core/manager/automodel_manager.py
+-rw-r--r--   0        0        0      554 2023-04-19 08:03:49.436991 optipack-0.0.19.dev0/optipack/core/manager/run_manager.py
+-rw-r--r--   0        0        0     2251 2023-03-20 10:11:52.420417 optipack-0.0.19.dev0/optipack/core/typing.py
+-rw-r--r--   0        0        0      143 2023-04-19 08:04:07.778785 optipack-0.0.19.dev0/optipack/core/visualizer/__init__.py
+-rw-r--r--   0        0        0      250 2023-03-30 10:37:47.836408 optipack-0.0.19.dev0/optipack/core/visualizer/base.py
+-rw-r--r--   0        0        0     4272 2023-04-19 08:27:30.465768 optipack-0.0.19.dev0/optipack/core/visualizer/otp_visualizer.py
+-rw-r--r--   0        0        0     1040 2023-04-19 08:04:46.367924 optipack-0.0.19.dev0/optipack/internal_utils/file_util.py
+-rw-r--r--   0        0        0     3775 2023-03-21 10:03:49.090579 optipack-0.0.19.dev0/optipack/internal_utils/terminal_util.py
+-rw-r--r--   0        0        0      155 2023-04-10 10:17:01.113759 optipack-0.0.19.dev0/optipack/sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 05:14:38.498269 optipack-0.0.19.dev0/optipack/sdk/optipack_env_controller.py
+-rw-r--r--   0        0        0     1062 2023-04-19 04:45:25.414500 optipack-0.0.19.dev0/optipack/sdk/optipack_init.py
+-rw-r--r--   0        0        0     4111 2023-04-20 11:09:12.936344 optipack-0.0.19.dev0/optipack/sdk/optipack_logger.py
+-rw-r--r--   0        0        0     6091 2023-04-19 04:46:45.842724 optipack-0.0.19.dev0/optipack/sdk/optipack_project_generator.py
+-rw-r--r--   0        0        0      158 2023-02-23 08:07:04.463928 optipack-0.0.19.dev0/optipack/sdk/optipack_run.py
+-rw-r--r--   0        0        0      249 2023-04-19 04:47:24.388598 optipack-0.0.19.dev0/optipack/sdk/optipack_utils.py
+-rw-r--r--   0        0        0      513 2023-04-21 08:58:04.734461 optipack-0.0.19.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 optipack-0.0.19.dev0/setup.py
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 optipack-0.0.19.dev0/PKG-INFO
```

### Comparing `optipack-0.0.18.dev0/LICENSE` & `optipack-0.0.19.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/README.md` & `optipack-0.0.19.dev0/README.md`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/.DS_Store` & `optipack-0.0.19.dev0/optipack/.DS_Store`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/.config/connection_config.yaml` & `optipack-0.0.19.dev0/optipack/.config/connection_config.yaml`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/.config/hyperparam_config.yaml` & `optipack-0.0.19.dev0/optipack/.config/hyperparam_config.yaml`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/asset/.DS_Store` & `optipack-0.0.19.dev0/optipack/asset/.DS_Store`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/asset/logo-large.png` & `optipack-0.0.19.dev0/optipack/asset/logo-large.png`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/asset/logo-small.png` & `optipack-0.0.19.dev0/optipack/asset/logo-small.png`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/cli.py` & `optipack-0.0.19.dev0/optipack/cli.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/core/automl/builder/base.py` & `optipack-0.0.19.dev0/optipack/core/automl/builder/base.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/core/automl/builder/data_builder.py` & `optipack-0.0.19.dev0/optipack/core/automl/builder/data_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .base import DataBuilder
 from typing import Any
-from ....sdk.optipack_logger import OptipackLogger
+from optipack.core.automl.builder.base import DataBuilder
+from optipack.sdk.optipack_logger import OptipackLogger
 
 class TorchDefaultDataBuilder(DataBuilder): 
     def __init__(self, mode: str, cfg: dict) -> None:
         logger = OptipackLogger(
             name = 'torch-data-builder-logger', 
             log_dir = './.otp_log/'
         )
```

### Comparing `optipack-0.0.18.dev0/optipack/core/automl/builder/metric_builder.py` & `optipack-0.0.19.dev0/optipack/core/automl/builder/metric_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .base import MetricBuilder
-from ....sdk.optipack_logger import OptipackLogger
+from optipack.core.automl.builder.base import MetricBuilder
+from optipack.sdk.optipack_logger import OptipackLogger
 
 
 class TorchDefaultMetricBuilder(MetricBuilder):
     def __init__(self, cfg: dict) -> None:
         logger = OptipackLogger(name = 'torch-metric-builder-logger',
                                 log_dir = './.otp_log/')
         super().__init__(cfg = cfg, logger=logger )
```

### Comparing `optipack-0.0.18.dev0/optipack/core/automl/builder/model_builder.py` & `optipack-0.0.19.dev0/optipack/core/automl/builder/model_builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .base import ModelBuilder
-from ....sdk.optipack_logger import OptipackLogger
+from optipack.core.automl.builder.base import ModelBuilder
+from optipack.sdk.optipack_logger import OptipackLogger
 
 class TorchDefaultModelBuilder(ModelBuilder): 
     def __init__(self, mode: str, cfg: dict) -> None:
 
         logger = OptipackLogger(
             name = 'torch-model-builder-logger', 
             log_dir = './.otp_log/'
```

### Comparing `optipack-0.0.18.dev0/optipack/core/automl/runner/base.py` & `optipack-0.0.19.dev0/optipack/core/automl/runner/base.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/core/fileio/reader_misc.py` & `optipack-0.0.19.dev0/optipack/core/fileio/reader_misc.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/core/fileio/storage_io.py` & `optipack-0.0.19.dev0/optipack/core/fileio/storage_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,17 @@
     def write_json(self): 
         pass
 
     @abstractmethod
     def view(self): 
         pass
 
+    # @abstractmethod
+    # def write(self):
+    #     pass
 
 class MongoDBStore(Storage):
     def __init__(self, storage_name: str, **kwargs) -> None:
         super().__init__(storage_name, kwargs)
         self._validate()
         self.connection_string = f'mongodb://{self.username}:{self.password}@{self.host}/{self.db_name}/'
         self._connect()
@@ -200,18 +203,18 @@
         self._connect()
         
     def _validate(self):
         return super()._validate()
 
     def _connect(self):
         try:
-            from fs_gcsfs import GCSFS
-            self.fs = GCSFS(bucket_name= self.bucket_name)
+            import fs_gcsfs
+            self.fs = fs_gcsfs.GCSFS(bucket_name= self.bucket)
         except Exception as e:
-            logger.error(f'Error {e} happened when initialize with bucket {self.bucket_name}') 
+            logger.error(f'Error {e} happened when initialize with bucket {self.bucket}') 
             raise e
     
     def write_json(self, path: str, content: dict):
         import json
         try: 
             with self.fs.open(path, 'w') as f:
                 f.write(json.dumps(content))
@@ -254,15 +257,15 @@
             return image
         except Exception as e:
             logger.error(e)
             raise e
 
 
 if __name__=='__main__': 
-    cfg = dict(bucket_name = 'om-mlops-serving-results-np')
+    cfg = dict(bucket = 'om-mlops-serving-results-np')
 
     store = Storage(storage_name='gcsfs', **cfg)
     # store.write_json('test_sdk.json',dict(id='test-sdk'))
     img = store.read_image('0.jpeg')
     print(img)
```

### Comparing `optipack-0.0.18.dev0/optipack/core/fileio/writer_misc.py` & `optipack-0.0.19.dev0/optipack/core/fileio/writer_misc.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/core/logger/base.py` & `optipack-0.0.19.dev0/optipack/core/logger/base.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/core/logger/otp_logger.py` & `optipack-0.0.19.dev0/optipack/core/logger/otp_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-from .base import BaseLogger
-
+from optipack.core.logger.base import BaseLogger
+import logging
 
 class SplunkLogger(BaseLogger):
     def __init__(self,
                  name: str,
+                 level: int = logging.DEBUG, 
                  config_path: str = 'core/logger/logger.cfg',
                  splunk_cfg: str = ''):
         super().__init__(name, config_path)
 
     def add_splunk_handler(self):
         # no token available
         raise NotImplementedError('Gimme token!!')
 
 
 class FileLogger(BaseLogger):
     def __init__(self,
                  name: str,
                  mode: str = 'w',
+                 level: int = logging.DEBUG,
                  log_dir: str = './log',
                  config_path: str = 'core/logger/logger.cfg'
                  ):
         super().__init__(name, config_path)
         self.log_dir = log_dir
         self.mode = mode
         self.add_file_handler()
+        if level != logging.DEBUG: 
+            self._logger.setLevel(level)
 
     def __set_log_path(self):
         import os
         try:
             if not os.path.exists(self.log_dir):
                 os.mkdir(self.log_dir)
             return os.path.join(self.log_dir, f'{self.name}.log')
@@ -39,15 +43,16 @@
         try:
             log_path = self.__set_log_path()
             file_handler = logging.FileHandler(log_path, mode=self.mode)
             file_handler.setFormatter(self._formatter)
             self._logger.addHandler(file_handler)
         except Exception as e:
             raise RuntimeError('Cannot create file handler')
-
+        
+    
 
 if __name__ == '__main__':
     logger = BaseLogger(name='base-logger').logger
     logger.debug('hello there')
     logger.warning('hello you')
 
     file_logger = FileLogger(name='file-logger').logger
```

### Comparing `optipack-0.0.18.dev0/optipack/core/manager/automl_manager.py` & `optipack-0.0.19.dev0/optipack/core/manager/automl_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,37 +5,38 @@
 
 class AutoML(): 
     def __init__(self, 
         mode: str,
         library: str,
         config_dir:str, 
     ) -> None:
-    
-        from automl.trainer import Trainer
-        from automl.evaluator import Evaluator
-        from automl.inferer import Inferer
-        from sdk.optipack_logger import OptipackLogger
-
-        self.logger = OptipackLogger(
-            name = 'automl', 
-            log_dir= './log'
-        )
-
-        mode_mapping = dict(
-            train = Trainer,
-            eval = Evaluator, 
-            infer = Inferer
-        )
-
-        try: 
-            RunnerCls = mode_mapping.get(mode, None)
-            assert RunnerCls, 'Invalid Runner class' 
-            self.auto_runner = RunnerCls(config_dir, library)
-        except Exception as e:
-            self.logger.error(e)
+        ...
+        # needs updating after AutoModel
+        # from optipack.core.automl.runner import Trainer
+        # from automl.evaluator import Evaluator
+        # from automl.inferer import Inferer
+        # from sdk.optipack_logger import OptipackLogger
+
+        # self.logger = OptipackLogger(
+        #     name = 'automl', 
+        #     log_dir= './log'
+        # )
+
+        # mode_mapping = dict(
+        #     train = Trainer,
+        #     eval = Evaluator, 
+        #     infer = Inferer
+        # )
+
+        # try: 
+        #     RunnerCls = mode_mapping.get(mode, None)
+        #     assert RunnerCls, 'Invalid Runner class' 
+        #     self.auto_runner = RunnerCls(config_dir, library)
+        # except Exception as e:
+        #     self.logger.error(e)
 
     def build(): 
         ...
 
     def run(): 
         ...
```

### Comparing `optipack-0.0.18.dev0/optipack/core/manager/automodel_manager.py` & `optipack-0.0.19.dev0/optipack/core/manager/automodel_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import List, Dict
-from ...sdk.optipack_logger import OptipackLogger
-from ..automl import builder
+from optipack.sdk.optipack_logger import OptipackLogger
+from optipack.core.automl import builder
 try:
     from typing import Self
 except:
     from typing_extensions import Self
 
 logger = OptipackLogger(name='default-logger', log_dir='./.opt_log/')
```

### Comparing `optipack-0.0.18.dev0/optipack/core/manager/run_manager.py` & `optipack-0.0.19.dev0/optipack/core/manager/run_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from abc import ABC, abstractmethod
 from fastcore.dispatch import *
-from . import core
+from optipack.core.automl import *
 from typing import Self
 
 class RunManager(): 
     def __new__(cls: type[Self]
         ) -> Self:
         
         
     
         return super().__new__()
 
     def __init__(self) -> None:
         super().__init__()
 
     @typedispatch
-    def run(self, trainer: core.automl.trainer.Trainer): 
+    def run(self, trainer: trainer.Trainer): 
         ...
 
     @typedispatch
-    def run(self, evaluator: core.automl.evaluator.Evaluator): 
+    def run(self, evaluator: evaluator.Evaluator): 
         ...
 
     @typedispatch
-    def run(self, inferer: core.automl.inferer.Inferer): 
+    def run(self, inferer: inferer.Inferer): 
         ...
```

### Comparing `optipack-0.0.18.dev0/optipack/core/typing.py` & `optipack-0.0.19.dev0/optipack/core/typing.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/core/visualizer/otp_visualizer.py` & `optipack-0.0.19.dev0/optipack/core/visualizer/otp_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 The wrapper for visualizers so that you can visualize metrics and scalars within simple logger command
 
 Raises:
     RuntimeError: _description_
     NotImplementedError: _description_
 """
 
-from .base import BaseVisualizer
+from optipack.core.visualizer.base import BaseVisualizer
 from fastcore.dispatch import *
-from .. import typing
+from optipack import typing
 
 
 class TensorboardVisualizer(BaseVisualizer):
     """Tensorboard that maps with normal logger
         Supported visualization: 
             - scalar
             - image
@@ -68,14 +68,15 @@
 
         try:
             executor = ThreadPoolExecutor()
             wait([executor.submit(self._log_tb, [m, metrics[m]])
                   for m in metrics
                   ])
             self.__writer.flush()
+            executor.shutdown()
         except Exception as e:
             raise RuntimeError(
                 f'Error {e} happened while attempting threading execution')
 
     @typedispatch
     def _log_tb(self, tag: str, scalar: float):
         self.__writer.add_scalar(tag, scalar, self._step)
```

### Comparing `optipack-0.0.18.dev0/optipack/internal_utils/file_util.py` & `optipack-0.0.19.dev0/optipack/internal_utils/file_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..core.fileio.reader_misc import read_yaml
+from optipack.core.fileio.reader_misc import read_yaml
 
 def environment_setup(appstart_file: str ='.config/app_start.yaml') -> bool:
 
     import os
     reset_after_run = False
 
     try:
```

### Comparing `optipack-0.0.18.dev0/optipack/internal_utils/terminal_util.py` & `optipack-0.0.19.dev0/optipack/internal_utils/terminal_util.py`

 * *Files identical despite different names*

### Comparing `optipack-0.0.18.dev0/optipack/sdk/optipack_logger.py` & `optipack-0.0.19.dev0/optipack/sdk/optipack_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # user -> get optipack log or model's log
 # adapter to use visualizer while logging
 
 import logging
-from ..core.logger import *
-from ..core.visualizer import *
+from optipack.core.logger import *
+from optipack.core.visualizer import *
 from typing import Any, MutableMapping, Mapping
 
-
 class OptipackLogger(logging.LoggerAdapter):
     def __init__(self,
                  name: str,
                  logger: str = 'file',
                  visualizer: str = '',
                  log_dir: str = '.',
                  extra: Mapping[str, object] = {},
+                 logger_kwargs: dict = {'level': logging.DEBUG},
                  visualizer_kwargs: dict = {'root_dir':'', 'run_folder': '', 'directory_list': {}}
                  ) -> None:
         '''Logger adapter that connect logger and visualizer.
 
         Args:
             name (str): logger's name. .log file will have the same name.
             logger (str, optional): type of logger, including "console","file". Defaults to "file".
@@ -43,15 +43,15 @@
 
         if not os.path.exists(log_dir):
             os.mkdir(log_dir)
         self._epoch = 0
         try:
             LogCls = LOGGER_MAPPER.get(logger, None)
             assert LogCls, 'Invalid logger class'
-            logger = LogCls(name=name, log_dir=log_dir).logger
+            logger = LogCls(name=name, log_dir=log_dir, **logger_kwargs).logger
         except:
             raise RuntimeError('Unable to initialize logger')
         
         try:
             VisCls = VISUALIZER_MAPPER.get(visualizer, None)
             assert VisCls, 'No visualizer provided'
             if not visualizer_kwargs:
```

### Comparing `optipack-0.0.18.dev0/optipack/sdk/optipack_project_generator.py` & `optipack-0.0.19.dev0/optipack/sdk/optipack_project_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 # logger
                 print(f'Exist inner path {path}')
                 return True 
         return False
 
     def _generate_folder_structure(self): 
         
-        from core.fileio.reader_misc import read_yaml
+        from optipack.core.fileio.reader_misc import read_yaml
 
         proj_struct_cfg_path = os.environ.get('PROJECT_STRUCTURE', '')
         assert proj_struct_cfg_path, 'Empty project structure path'
         
         self._structure_dir = os.path.join(self._optipack_path, proj_struct_cfg_path)
         fs = read_yaml(self._structure_dir)
         self._folder_structure = fs.get('project_structure', [])
@@ -79,28 +79,28 @@
             new_dir = os.path.join(parent_dir, folder)
             if not os.path.exists(new_dir):
                 os.mkdir(new_dir)
         self.__recursive_gen_folder(parent_dir, folder_structure)
 
     def _generate_configs_files(self): 
         
-        from core.fileio.reader_misc import read_yaml
+        from optipack.core.fileio.reader_misc import read_yaml
         
         for path in self.__cfg_gen_mapper: 
             cfg_path = os.environ.get(path, '')    
             assert cfg_path, f'Empty {path} config path'
             cfg_path = os.path.join(self._optipack_path, cfg_path)
             cfg_dict = read_yaml(cfg_path)
             func = self.__cfg_gen_mapper.get(path)
             # print(f'Writing {path}')
             func(cfg_dict)
 
     def __generate_connection_configs(self, cfg_dict): 
 
-        from core.fileio.reader_misc import write_yaml
+        from optipack.core.fileio.reader_misc import write_yaml
         
         root_dir = os.path.join(self._parent_dir, cfg_dict.get('root_dir', ''))
         assert root_dir, 'Empty connection root dir'
         folder = cfg_dict.get('folder', '')
         assert folder, 'Empty connection folder'
 
         cfg_dir = os.path.join(root_dir, folder)
@@ -128,15 +128,15 @@
             assert inner_dict, f'Empty {tool_name} {key}'
             out_dict[key] = inner_dict.get(self._env)
             del cfg_dict[key]
         out_dict.update(cfg_dict)
         return out_dict
     
     def __generate_hyperparam_configs(self, cfg_dict): 
-        from core.fileio.reader_misc import write_yaml
+        from optipack.core.fileio.reader_misc import write_yaml
         
         root_dir = os.path.join(self._parent_dir, cfg_dict.get('root_dir', ''))
         assert root_dir, 'Empty hyperparameters root dir'
         folder = cfg_dict.get('folder', '')
         assert folder, 'Empty hyperparameters folder'
 
         cfg_dir = os.path.join(root_dir, folder)
@@ -149,15 +149,15 @@
         for cfg_name in hyperparam_cfg: 
             cfg_path = os.path.join(cfg_dir, f'{cfg_name}.yaml')
             cfg = hyperparam_cfg.get(cfg_name, {})
             assert cfg, f'Empty {cfg_name} configs'
             write_yaml(cfg_path, cfg)
     
     def __copy_file(self, cfg_dict): 
-        from core.fileio.writer_misc import write_yaml
+        from optipack.core.fileio.writer_misc import write_yaml
 
         root_dir = os.path.join(self._parent_dir, cfg_dict.get('root_dir', ''))
         assert root_dir, 'Empty run config root dir'
         
         cfg_dir = os.path.join(root_dir, f'run_config.yaml')
         cfg = cfg_dict.get('config', {})
         assert cfg, 'Empty run config'
```

### Comparing `optipack-0.0.18.dev0/setup.py` & `optipack-0.0.19.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,31 +13,37 @@
  'optipack.internal_utils',
  'optipack.sdk']
 
 package_data = \
 {'': ['*'], 'optipack': ['.config/*', 'asset/*']}
 
 install_requires = \
-['Pillow==9.4.0', 'pyyaml==6.0', 'rich==13.3.1', 'typer>=0.7.0,<0.8.0']
+['Pillow==9.4.0',
+ 'fs-gcsfs>=1.5.1,<2.0.0',
+ 'matplotlib>=3.7.1,<4.0.0',
+ 'pyyaml==6.0',
+ 'rich==13.3.1',
+ 'torch>=2.0.0,<3.0.0',
+ 'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['optipack = optipack.__main__:start']}
 
 setup_kwargs = {
     'name': 'optipack',
-    'version': '0.0.18.dev0',
+    'version': '0.0.19.dev0',
     'description': 'The optimal ML package',
     'long_description': "![optipack](asset/image/logo.png)\n\n# What optipack do: \n- Workspace management: \n    - Generate folder structure for ML project \n    - Generate files following the given environment in yaml format, including: \n        - tool connection configuration \n        - hyperparameter configuration \n        - model run config\n-  Logging: 🔥 all-in-one logger\n    - Support console/file logger for users' log! 🔥 No more uggly print, no more terminal scrolling\n    - Support tensorboard metric log. \n\n# Installation:  \n## 1. Installation from PYPI: \n- Run `pip install optipack`\n## 2. Installation from source: \n- Clone this repo \n- Change directory to optipack\n- Run `pip install . `\n\n# How to use: \n## 1. Use as CLI \n- All you need is running `optipack` on terminal :) \n\n## 2. Use as library\n- ... ",
     'author': 'indigoYoshimaru',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3,<4',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `optipack-0.0.18.dev0/PKG-INFO` & `optipack-0.0.19.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: optipack
-Version: 0.0.18.dev0
+Version: 0.0.19.dev0
 Summary: The optimal ML package
 Author: indigoYoshimaru
-Requires-Python: >=3,<4
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (==9.4.0)
+Requires-Dist: fs-gcsfs (>=1.5.1,<2.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pyyaml (==6.0)
 Requires-Dist: rich (==13.3.1)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 ![optipack](asset/image/logo.png)
 
 # What optipack do: 
 - Workspace management:
```

