# Comparing `tmp/xh-cpu-usage-simulator-0.1.2.tar.gz` & `tmp/xh-cpu-usage-simulator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-cpu-usage-simulator-0.1.2.tar", last modified: Wed Apr 19 16:39:58 2023, max compression
+gzip compressed data, was "xh-cpu-usage-simulator-0.1.3.tar", last modified: Fri Apr 21 00:57:03 2023, max compression
```

## Comparing `xh-cpu-usage-simulator-0.1.2.tar` & `xh-cpu-usage-simulator-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:39:58.260895 xh-cpu-usage-simulator-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-19 16:39:44.000000 xh-cpu-usage-simulator-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 16:39:58.260895 xh-cpu-usage-simulator-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 16:39:44.000000 xh-cpu-usage-simulator-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-19 16:39:44.000000 xh-cpu-usage-simulator-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:39:58.260895 xh-cpu-usage-simulator-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:39:58.256894 xh-cpu-usage-simulator-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:39:58.260895 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 16:39:44.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 16:39:44.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/MovingAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 16:39:44.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/PsMonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-19 16:39:44.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/TaskWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 16:39:44.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/TestMovingAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-19 16:39:44.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:39:58.260895 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-19 16:39:58.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 16:39:58.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:39:58.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 16:39:58.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 16:39:58.000000 xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:57:03.931194 xh-cpu-usage-simulator-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-21 00:56:51.000000 xh-cpu-usage-simulator-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-21 00:57:03.931194 xh-cpu-usage-simulator-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-21 00:56:51.000000 xh-cpu-usage-simulator-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-21 00:56:51.000000 xh-cpu-usage-simulator-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:57:03.931194 xh-cpu-usage-simulator-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:57:03.927194 xh-cpu-usage-simulator-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:57:03.931194 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-21 00:56:51.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-21 00:56:51.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/MovingAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 00:56:51.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/PsMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-21 00:56:51.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/TaskWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-21 00:56:51.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/TestMovingAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-21 00:56:51.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:57:03.931194 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-21 00:57:03.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-21 00:57:03.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:57:03.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 00:57:03.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 00:57:03.000000 xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator.egg-info/top_level.txt
```

### Comparing `xh-cpu-usage-simulator-0.1.2/LICENSE.txt` & `xh-cpu-usage-simulator-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.2/PKG-INFO` & `xh-cpu-usage-simulator-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-cpu-usage-simulator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools simulating the cpu usage
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-cpu-usage-simulator-0.1.2/pyproject.toml` & `xh-cpu-usage-simulator-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-cpu-usage-simulator"
-version = "0.1.2"
+version = "0.1.3"
 description = "Tools simulating the cpu usage"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "psutil==5.9.5", "scikit-learn==1.2.2", "numpy==1.24.2",]
 [[project.authors]]
 name = "xethhung"
```

### Comparing `xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py` & `xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/LinearRegressionPrediction.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/MovingAvg.py` & `xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/MovingAvg.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/TaskWorker.py` & `xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/TaskWorker.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/TestMovingAvg.py` & `xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/TestMovingAvg.py`

 * *Files identical despite different names*

### Comparing `xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator/__main__.py` & `xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,18 @@
                         f"{rounds:05d}::Targeting[{lower_bound} < {target} < {upper_bound}], now[{m_avg.avg}], increase operation with loading[{cur_total_mv}] from {cur_total_operation} to {new_total_operation}")
                 elif upper_bound < m_avg.avg:
                     for i in d:
                         n_op = next_operation()
                         d[i] = n_op / len(d) if n_op is not None else d[i] * 0.85
                     new_total_operation = round(sum([d[i] for i in d]), 2)
                     print(
-                        f"{rounds:05d}Targeting[{lower_bound} < {target} < {upper_bound}], now[{m_avg.avg}], decrease operation with loading[{cur_total_mv}] from {cur_total_operation} to {new_total_operation}")
+                        f"{rounds:05d}::Targeting[{lower_bound} < {target} < {upper_bound}], now[{m_avg.avg}], decrease operation with loading[{cur_total_mv}] from {cur_total_operation} to {new_total_operation}")
                 else:
                     for i in d:
                         n_op = next_operation()
                         d[i] = n_op / len(d) if n_op is not None else d[i] * 0.85
                     new_total_operation = round(sum([d[i] for i in d]), 2)
                     print(
-                        f"{rounds:05d}Targeting[{lower_bound} < {target} < {upper_bound}], now[{m_avg.avg}], adjustment with loading[{cur_total_mv}] from {cur_total_operation} to {new_total_operation}")
+                        f"{rounds:05d}::Targeting[{lower_bound} < {target} < {upper_bound}], now[{m_avg.avg}], adjustment with loading[{cur_total_mv}] from {cur_total_operation} to {new_total_operation}")
         m_avg.insert(m.avg)
 
 # See PyCharm help at https://www.jetbrains.com/help/pycharm/
```

### Comparing `xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator.egg-info/PKG-INFO` & `xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-cpu-usage-simulator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools simulating the cpu usage
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-cpu-usage-simulator-0.1.2/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt` & `xh-cpu-usage-simulator-0.1.3/src/xh_cpu_usage_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

