# Comparing `tmp/hcai-nova-server-nightly-0.1.3.dev202304201558.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.3.dev202304201601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.3.dev202304201558.tar", last modified: Thu Apr 20 15:58:10 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.3.dev202304201601.tar", last modified: Thu Apr 20 16:01:12 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558.tar` & `hcai-nova-server-nightly-0.1.3.dev202304201601.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 15:58:10.759003 hcai-nova-server-nightly-0.1.3.dev202304201558/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-04-20 15:58:10.759003 hcai-nova-server-nightly-0.1.3.dev202304201558/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 15:58:10.755003 hcai-nova-server-nightly-0.1.3.dev202304201558/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-04-20 15:58:10.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-20 15:58:10.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 15:58:10.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-20 15:58:10.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-20 15:58:10.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 15:58:10.755003 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 15:58:10.755003 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/logs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/nova_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 15:58:10.759003 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     8601 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7845 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 15:58:10.759003 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 15:58:10.759003 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10762 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 15:58:10.759003 hcai-nova-server-nightly-0.1.3.dev202304201558/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-04-20 15:57:56.000000 hcai-nova-server-nightly-0.1.3.dev202304201558/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 16:01:12.910226 hcai-nova-server-nightly-0.1.3.dev202304201601/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-04-20 16:01:12.910226 hcai-nova-server-nightly-0.1.3.dev202304201601/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 16:01:12.910226 hcai-nova-server-nightly-0.1.3.dev202304201601/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-04-20 16:01:12.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-20 16:01:12.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 16:01:12.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-20 16:01:12.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-20 16:01:12.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 16:01:12.910226 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 16:01:12.910226 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/logs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/nova_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 16:01:12.910226 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8601 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7845 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 16:01:12.910226 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 16:01:12.910226 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10762 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 16:01:12.910226 hcai-nova-server-nightly-0.1.3.dev202304201601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-04-20 16:00:59.000000 hcai-nova-server-nightly-0.1.3.dev202304201601/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/PKG-INFO` & `hcai-nova-server-nightly-0.1.3.dev202304201601/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.3.dev202304201558
+Version: 0.1.3.dev202304201601
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/README.md` & `hcai-nova-server-nightly-0.1.3.dev202304201601/README.md`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.3.dev202304201601/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.3.dev202304201558
+Version: 0.1.3.dev202304201601
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.3.dev202304201601/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/nova_backend.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/nova_backend.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/predict.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202304201558/setup.py` & `hcai-nova-server-nightly-0.1.3.dev202304201601/setup.py`

 * *Files identical despite different names*

