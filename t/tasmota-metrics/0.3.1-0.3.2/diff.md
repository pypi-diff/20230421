# Comparing `tmp/tasmota-metrics-0.3.1.tar.gz` & `tmp/tasmota-metrics-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasmota-metrics-0.3.1.tar", last modified: Fri Apr 21 09:44:42 2023, max compression
+gzip compressed data, was "tasmota-metrics-0.3.2.tar", last modified: Fri Apr 21 09:58:04 2023, max compression
```

## Comparing `tasmota-metrics-0.3.1.tar` & `tasmota-metrics-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:44:42.603522 tasmota-metrics-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-21 09:44:42.603522 tasmota-metrics-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 09:44:42.603522 tasmota-metrics-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:44:42.599521 tasmota-metrics-0.3.1/tasmota_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/tasmota_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/tasmota_metrics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:44:42.603522 tasmota-metrics-0.3.1/tasmota_metrics/chip_info/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32c2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32c3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32c6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32h2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32h4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32s2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32s3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:44:42.599521 tasmota-metrics-0.3.1/tasmota_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-21 09:44:42.000000 tasmota-metrics-0.3.1/tasmota_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-21 09:44:42.000000 tasmota-metrics-0.3.1/tasmota_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:44:42.000000 tasmota-metrics-0.3.1/tasmota_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 09:44:42.000000 tasmota-metrics-0.3.1/tasmota_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 09:44:42.000000 tasmota-metrics-0.3.1/tasmota_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:44:42.603522 tasmota-metrics-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 09:44:23.000000 tasmota-metrics-0.3.1/test/test_tasmota_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:58:04.364274 tasmota-metrics-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-21 09:58:04.364274 tasmota-metrics-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 09:58:04.364274 tasmota-metrics-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:58:04.356273 tasmota-metrics-0.3.2/tasmota_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:58:04.364274 tasmota-metrics-0.3.2/tasmota_metrics/chip_info/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32c2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32c6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32h2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32h4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32s2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32s3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    56582 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/tasmota_metrics/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:58:04.360273 tasmota-metrics-0.3.2/tasmota_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-21 09:58:04.000000 tasmota-metrics-0.3.2/tasmota_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-21 09:58:04.000000 tasmota-metrics-0.3.2/tasmota_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:58:04.000000 tasmota-metrics-0.3.2/tasmota_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 09:58:04.000000 tasmota-metrics-0.3.2/tasmota_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 09:58:04.000000 tasmota-metrics-0.3.2/tasmota_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:58:04.364274 tasmota-metrics-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 09:57:45.000000 tasmota-metrics-0.3.2/test/test_tasmota_metrics.py
```

### Comparing `tasmota-metrics-0.3.1/LICENSE` & `tasmota-metrics-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.1/PKG-INFO` & `tasmota-metrics-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tasmota-metrics
-Version: 0.3.1
+Version: 0.3.2
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/jasons2866/tasmota-metrics
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tasmota-metrics-0.3.1/setup.py` & `tasmota-metrics-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32.yaml` & `tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32.yaml`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32s2.yaml` & `tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32s2.yaml`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.1/tasmota_metrics/chip_info/esp32s3.yaml` & `tasmota-metrics-0.3.2/tasmota_metrics/chip_info/esp32s3.yaml`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.1/tasmota_metrics.egg-info/PKG-INFO` & `tasmota-metrics-0.3.2/tasmota_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tasmota-metrics
-Version: 0.3.1
+Version: 0.3.2
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/jasons2866/tasmota-metrics
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tasmota-metrics-0.3.1/tasmota_metrics.egg-info/SOURCES.txt` & `tasmota-metrics-0.3.2/tasmota_metrics.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 tasmota_metrics/__init__.py
 tasmota_metrics/__main__.py
+tasmota_metrics/core.py
 tasmota_metrics.egg-info/PKG-INFO
 tasmota_metrics.egg-info/SOURCES.txt
 tasmota_metrics.egg-info/dependency_links.txt
 tasmota_metrics.egg-info/requires.txt
 tasmota_metrics.egg-info/top_level.txt
 tasmota_metrics/chip_info/esp32.yaml
 tasmota_metrics/chip_info/esp32c2.yaml
```

### Comparing `tasmota-metrics-0.3.1/test/test_tasmota_metrics.py` & `tasmota-metrics-0.3.2/test/test_tasmota_metrics.py`

 * *Files identical despite different names*

