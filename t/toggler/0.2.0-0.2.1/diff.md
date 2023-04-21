# Comparing `tmp/toggler-0.2.0.tar.gz` & `tmp/toggler-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toggler-0.2.0.tar", last modified: Thu Apr 20 05:32:34 2023, max compression
+gzip compressed data, was "toggler-0.2.1.tar", last modified: Fri Apr 21 05:28:45 2023, max compression
```

## Comparing `toggler-0.2.0.tar` & `toggler-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.001540 toggler-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-20 05:32:25.000000 toggler-0.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-20 05:32:25.000000 toggler-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-20 05:32:25.000000 toggler-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 05:32:25.000000 toggler-0.2.0/.python-black
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-20 05:32:34.005540 toggler-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-20 05:32:25.000000 toggler-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 05:32:25.000000 toggler-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-20 05:32:34.005540 toggler-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-20 05:32:25.000000 toggler-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:25.000000 toggler-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-20 05:32:25.000000 toggler-0.2.0/tests/data/cfg_1.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-20 05:32:25.000000 toggler-0.2.0/tests/test_config_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-20 05:32:25.000000 toggler-0.2.0/tests/test_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/toggler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/toggler/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/services/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/toggler.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/toggler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-20 05:32:33.000000 toggler-0.2.0/toggler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-20 05:32:33.000000 toggler-0.2.0/toggler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 05:32:33.000000 toggler-0.2.0/toggler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 05:32:33.000000 toggler-0.2.0/toggler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 05:32:33.000000 toggler-0.2.0/toggler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 05:32:25.000000 toggler-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:45.696311 toggler-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:45.692311 toggler-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:45.696311 toggler-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-21 05:28:36.000000 toggler-0.2.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 05:28:36.000000 toggler-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-21 05:28:36.000000 toggler-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 05:28:36.000000 toggler-0.2.1/.python-black
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-21 05:28:45.696311 toggler-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-21 05:28:36.000000 toggler-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 05:28:36.000000 toggler-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-21 05:28:45.696311 toggler-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-21 05:28:36.000000 toggler-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:45.696311 toggler-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:36.000000 toggler-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:45.696311 toggler-0.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-21 05:28:36.000000 toggler-0.2.1/tests/data/cfg_1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-21 05:28:36.000000 toggler-0.2.1/tests/test_config_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-21 05:28:36.000000 toggler-0.2.1/tests/test_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:45.696311 toggler-0.2.1/toggler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:36.000000 toggler-0.2.1/toggler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-21 05:28:36.000000 toggler-0.2.1/toggler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-21 05:28:36.000000 toggler-0.2.1/toggler/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:45.696311 toggler-0.2.1/toggler/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:36.000000 toggler-0.2.1/toggler/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-21 05:28:36.000000 toggler-0.2.1/toggler/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-21 05:28:36.000000 toggler-0.2.1/toggler/services/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-21 05:28:36.000000 toggler-0.2.1/toggler/toggler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-21 05:28:36.000000 toggler-0.2.1/toggler/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:28:45.696311 toggler-0.2.1/toggler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-21 05:28:45.000000 toggler-0.2.1/toggler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-21 05:28:45.000000 toggler-0.2.1/toggler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 05:28:45.000000 toggler-0.2.1/toggler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 05:28:45.000000 toggler-0.2.1/toggler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 05:28:45.000000 toggler-0.2.1/toggler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-21 05:28:36.000000 toggler-0.2.1/tox.ini
```

### Comparing `toggler-0.2.0/.github/workflows/main.yml` & `toggler-0.2.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `toggler-0.2.0/.pre-commit-config.yaml` & `toggler-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `toggler-0.2.0/PKG-INFO` & `toggler-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,44 @@
-Metadata-Version: 2.1
-Name: toggler
-Version: 0.2.0
-Summary: Feature Flags Manager
-Home-page: https://github.com/versada/toggler
-Author: Versada (Andrius Laukavičius)
-Author-email: andrius.laukavicius@versada.eu
-License: LGPLv3
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Description-Content-Type: text/markdown
-Provides-Extra: test
-
 # Toggler
 
 Toggler allows to set up feature toggles (flags) on a YAML file and validate whether
 specific flag is ON or OFF on specific environment.
 
 ## How to Use
 
 ### Configure Feature Toggles
 
 Feature toggles are configured in `yaml` file:
 
 ```yaml
 ---
-prod:
-  feature2:
-    active: true
-stage:
-  feature1:
-    active: true
-    ref: r123
-    deadline: 2022-01-01
-  feature2:
-    active: true
-  feature3:
-    active: false
+feature1:
+  modes: [prod, stage]
+  date: 2023-01-01
+  days_to_expire: 10
+  ref: r123
+feature2:
+  modes: [stage]
+  date: 2023-01-01
+feature3:
+  modes: [other]
+  date: 2023-01-01
 ```
 
 Structure:
 
-* modes (e.g prod, stage), defines features defined on specific mode.
+* modes (e.g prod, stage), defines features enabled on specific mode.
 * features (e.g feature1, feature2) are feature names used to identify which
   feature is used or not:
     - active: whether feature is enabled or not. If feature is not defined on
       specific mode, it is implicitly treated as disabled. This is the only required field.
     - ref: reference to feature or ticket (for convenience).
-    - deadline: if set, will check if feature flag has been for too long and logs
-      a warning if its passed a deadline.
+    - date: when feature flag was added.
+    - days_to_expire: how many days feature flag is to stay. Warning logs will
+      be written after deadline.
 
 ### Define mode and config file path
 
 You can either explicitly initialize `Toggler` with its optional arguments, `mode` and `path` (or `stream`) or you can use environment variables `TOGGLER_MODE` and `TOGGLER_CFG`.
 
 For example:
 
@@ -80,15 +61,15 @@
 ```
 
 ### Using toggler in tests
 
 You can force toggle feature to make it easier to test.
 
 ```python
-from toggler.env import toggle_feature
+from toggler.services.env import toggle_feature
 
 
 def test_feature1_on():
     with toggle_feature("feature1", True):  # Force enable
         # test if feature1 logic works as expected
         ...
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `toggler-0.2.0/setup.py` & `toggler-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `toggler-0.2.0/tests/test_config_service.py` & `toggler-0.2.1/tests/test_config_service.py`

 * *Files identical despite different names*

### Comparing `toggler-0.2.0/tests/test_feature.py` & `toggler-0.2.1/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `toggler-0.2.0/toggler/model.py` & `toggler-0.2.1/toggler/model.py`

 * *Files identical despite different names*

### Comparing `toggler-0.2.0/toggler/services/config.py` & `toggler-0.2.1/toggler/services/config.py`

 * *Files identical despite different names*

### Comparing `toggler-0.2.0/toggler/services/env.py` & `toggler-0.2.1/toggler/services/env.py`

 * *Files identical despite different names*

### Comparing `toggler-0.2.0/toggler/toggler.py` & `toggler-0.2.1/toggler/toggler.py`

 * *Files identical despite different names*

### Comparing `toggler-0.2.0/toggler.egg-info/PKG-INFO` & `toggler-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toggler
-Version: 0.2.0
+Version: 0.2.1
 Summary: Feature Flags Manager
 Home-page: https://github.com/versada/toggler
 Author: Versada (Andrius Laukavičius)
 Author-email: andrius.laukavicius@versada.eu
 License: LGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -26,38 +26,38 @@
 
 ### Configure Feature Toggles
 
 Feature toggles are configured in `yaml` file:
 
 ```yaml
 ---
-prod:
-  feature2:
-    active: true
-stage:
-  feature1:
-    active: true
-    ref: r123
-    deadline: 2022-01-01
-  feature2:
-    active: true
-  feature3:
-    active: false
+feature1:
+  modes: [prod, stage]
+  date: 2023-01-01
+  days_to_expire: 10
+  ref: r123
+feature2:
+  modes: [stage]
+  date: 2023-01-01
+feature3:
+  modes: [other]
+  date: 2023-01-01
 ```
 
 Structure:
 
-* modes (e.g prod, stage), defines features defined on specific mode.
+* modes (e.g prod, stage), defines features enabled on specific mode.
 * features (e.g feature1, feature2) are feature names used to identify which
   feature is used or not:
     - active: whether feature is enabled or not. If feature is not defined on
       specific mode, it is implicitly treated as disabled. This is the only required field.
     - ref: reference to feature or ticket (for convenience).
-    - deadline: if set, will check if feature flag has been for too long and logs
-      a warning if its passed a deadline.
+    - date: when feature flag was added.
+    - days_to_expire: how many days feature flag is to stay. Warning logs will
+      be written after deadline.
 
 ### Define mode and config file path
 
 You can either explicitly initialize `Toggler` with its optional arguments, `mode` and `path` (or `stream`) or you can use environment variables `TOGGLER_MODE` and `TOGGLER_CFG`.
 
 For example:
 
@@ -80,15 +80,15 @@
 ```
 
 ### Using toggler in tests
 
 You can force toggle feature to make it easier to test.
 
 ```python
-from toggler.env import toggle_feature
+from toggler.services.env import toggle_feature
 
 
 def test_feature1_on():
     with toggle_feature("feature1", True):  # Force enable
         # test if feature1 logic works as expected
         ...
```

### Comparing `toggler-0.2.0/toggler.egg-info/SOURCES.txt` & `toggler-0.2.1/toggler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

