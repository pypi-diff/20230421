# Comparing `tmp/charmed-kubeflow-chisme-0.0.8.tar.gz` & `tmp/charmed-kubeflow-chisme-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmed-kubeflow-chisme-0.0.8.tar", last modified: Fri Mar 17 18:40:33 2023, max compression
+gzip compressed data, was "charmed-kubeflow-chisme-0.0.9.tar", last modified: Fri Apr 21 13:09:27 2023, max compression
```

## Comparing `charmed-kubeflow-chisme-0.0.8.tar` & `charmed-kubeflow-chisme-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,48 @@
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.167178 charmed-kubeflow-chisme-0.0.8/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)    11357 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/LICENSE
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1944 2023-03-17 18:40:33.167178 charmed-kubeflow-chisme-0.0.8/PKG-INFO
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1451 2023-03-17 18:39:58.000000 charmed-kubeflow-chisme-0.0.8/README.md
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1178 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/pyproject.toml
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      731 2023-03-17 18:40:33.167178 charmed-kubeflow-chisme-0.0.8/setup.cfg
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.159178 charmed-kubeflow-chisme-0.0.8/src/
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.159178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      147 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/__init__.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.163178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/bundle/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      174 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/bundle/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     3620 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/bundle/_bundle.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.163178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/exceptions/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      446 2023-03-17 18:39:58.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/exceptions/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      751 2023-03-17 18:39:58.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/exceptions/_generic_charm_runtime_error.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      374 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/exceptions/_kubernetes.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      953 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/exceptions/_with_status.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.163178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/juju/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      214 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/juju/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1597 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/juju/_juju.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.163178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/kubernetes/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      293 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/kubernetes/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     2464 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/kubernetes/_check_resources.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)    13325 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/kubernetes/_kubernetes_resource_handler.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      855 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/kubernetes/_validate_statefulset.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.163178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/lightkube/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      147 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/lightkube/__init__.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.163178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/lightkube/batch/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      237 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/lightkube/batch/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     3946 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/lightkube/batch/_many.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     2308 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/lightkube/batch/_sort_objects.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      761 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/lightkube/mocking.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.163178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/pebble/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      189 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/pebble/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1306 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/pebble/_update_layer.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.163178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/status_handling/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      235 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/status_handling/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      863 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/status_handling/_get_first_worst_error.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.163178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/types/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      345 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/types/__init__.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      461 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/types/_charm_status.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)      298 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/types/_lightkube.py
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.163178 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme.egg-info/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1944 2023-03-17 18:40:33.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme.egg-info/PKG-INFO
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1731 2023-03-17 18:40:33.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme.egg-info/SOURCES.txt
--rw-rw-r--   0 scribs    (1000) scribs    (1000)        1 2023-03-17 18:40:33.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme.egg-info/dependency_links.txt
--rw-rw-r--   0 scribs    (1000) scribs    (1000)       83 2023-03-17 18:40:33.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme.egg-info/requires.txt
--rw-rw-r--   0 scribs    (1000) scribs    (1000)       24 2023-03-17 18:40:33.000000 charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme.egg-info/top_level.txt
-drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-03-17 18:40:33.167178 charmed-kubeflow-chisme-0.0.8/tests/
--rw-rw-r--   0 scribs    (1000) scribs    (1000)    16051 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/tests/test_kubernetes.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     5065 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/tests/test_lightkube.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     2142 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/tests/test_pebble.py
--rw-rw-r--   0 scribs    (1000) scribs    (1000)     1663 2023-03-16 18:01:40.000000 charmed-kubeflow-chisme-0.0.8/tests/test_status_handling.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.542024 charmed-kubeflow-chisme-0.0.9/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)    11357 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/LICENSE
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     2230 2023-04-21 13:09:27.542024 charmed-kubeflow-chisme-0.0.9/PKG-INFO
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     1737 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/README.md
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     1178 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/pyproject.toml
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      741 2023-04-21 13:09:27.542024 charmed-kubeflow-chisme-0.0.9/setup.cfg
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.522024 charmed-kubeflow-chisme-0.0.9/src/
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.526024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      147 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/__init__.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.530024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/bundle/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      174 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/bundle/__init__.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     3620 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/bundle/_bundle.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.530024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      446 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/__init__.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      751 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/_generic_charm_runtime_error.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      374 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/_kubernetes.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      953 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/_with_status.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.534024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/juju/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      214 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/juju/__init__.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     1597 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/juju/_juju.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.534024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      364 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/__init__.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     2464 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_check_resources.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)    23458 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_kubernetes_resource_handler.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      855 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_validate_statefulset.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.538024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      147 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/__init__.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.538024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      237 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/__init__.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     3946 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/_many.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     2308 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/_sort_objects.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      761 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/mocking.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.538024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/pebble/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      189 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/pebble/__init__.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     1306 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/pebble/_update_layer.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.542024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/status_handling/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      235 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/status_handling/__init__.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      863 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/status_handling/_get_first_worst_error.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.542024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/types/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      422 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/types/__init__.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      461 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/types/_charm_status.py
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)      473 2023-04-21 12:57:23.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/types/_lightkube.py
+drwxrwxr-x   0 scribs    (1000) scribs    (1000)        0 2023-04-21 13:09:27.526024 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     2230 2023-04-21 13:09:27.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/PKG-INFO
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)     1631 2023-04-21 13:09:27.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/SOURCES.txt
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)        1 2023-04-21 13:09:27.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/dependency_links.txt
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)       92 2023-04-21 13:09:27.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/requires.txt
+-rw-rw-r--   0 scribs    (1000) scribs    (1000)       24 2023-04-21 13:09:27.000000 charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/top_level.txt
```

### Comparing `charmed-kubeflow-chisme-0.0.8/LICENSE` & `charmed-kubeflow-chisme-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/PKG-INFO` & `charmed-kubeflow-chisme-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmed-kubeflow-chisme
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of helpers for Charms maintained by the Charmed Kubeflow team
 Home-page: https://github.com/canonical/charmed-kubeflow-chisme
 Author: Charmed Kubeflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -30,9 +30,14 @@
 
 [ckf]: https://charmed-kubeflow.io/
 [lightkube-rtd]: https://lightkube.readthedocs.io/en/latest/
 
 # Publishing to PyPi
 
 To publish a new release to Pypi:
-1. Update [setup.cfg](https://github.com/canonical/charmed-kubeflow-chisme/blob/main/setup.cfg#L3) to the new version and commit it to the repo via a completed PR
-2. Pull the repo and use `tox -e publish` to publish
+1. Update [setup.cfg](https://github.com/canonical/charmed-kubeflow-chisme/blob/main/setup.cfg#L3) to the new version 
+   and commit it to the repo via a completed PR
+2. Apply local git tag according to the format `X.X.X` (semantic versioning) on the main branch
+3. Push tag to the repo. Example: `git push origin 0.0.8`
+4. GitHub Action will create a new release on GitHub
+5. Edit release via GitHub UI and click publish
+6. GitHub Action will automatically publish the same commit to PyPi repository
```

### Comparing `charmed-kubeflow-chisme-0.0.8/README.md` & `charmed-kubeflow-chisme-0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,9 +16,14 @@
 
 [ckf]: https://charmed-kubeflow.io/
 [lightkube-rtd]: https://lightkube.readthedocs.io/en/latest/
 
 # Publishing to PyPi
 
 To publish a new release to Pypi:
-1. Update [setup.cfg](https://github.com/canonical/charmed-kubeflow-chisme/blob/main/setup.cfg#L3) to the new version and commit it to the repo via a completed PR
-2. Pull the repo and use `tox -e publish` to publish
+1. Update [setup.cfg](https://github.com/canonical/charmed-kubeflow-chisme/blob/main/setup.cfg#L3) to the new version 
+   and commit it to the repo via a completed PR
+2. Apply local git tag according to the format `X.X.X` (semantic versioning) on the main branch
+3. Push tag to the repo. Example: `git push origin 0.0.8`
+4. GitHub Action will create a new release on GitHub
+5. Edit release via GitHub UI and click publish
+6. GitHub Action will automatically publish the same commit to PyPi repository
```

### Comparing `charmed-kubeflow-chisme-0.0.8/pyproject.toml` & `charmed-kubeflow-chisme-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/setup.cfg` & `charmed-kubeflow-chisme-0.0.9/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = charmed-kubeflow-chisme
-version = 0.0.8
+version = 0.0.9
 author = Charmed Kubeflow
 description = A collection of helpers for Charms maintained by the Charmed Kubeflow team
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/canonical/charmed-kubeflow-chisme
 classifiers = 
 	Programming Language :: Python :: 3
@@ -13,19 +13,20 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	deepdiff==6.2.1
+	deepdiff<=6.2.1
 	jinja2
 	lightkube > 0.10.0
 	ops > 1.2.0
 	ruamel.yaml
+	tenacity
 
 [options.extras_require]
 test = 
 	pytest
 	black
 
 [options.packages.find]
```

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/bundle/_bundle.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/bundle/_bundle.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/exceptions/_generic_charm_runtime_error.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/_generic_charm_runtime_error.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/exceptions/_with_status.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/exceptions/_with_status.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/juju/_juju.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/juju/_juju.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/kubernetes/_check_resources.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_check_resources.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/kubernetes/_validate_statefulset.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/kubernetes/_validate_statefulset.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/lightkube/batch/_many.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/_many.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/lightkube/batch/_sort_objects.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/batch/_sort_objects.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/lightkube/mocking.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/lightkube/mocking.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/pebble/_update_layer.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/pebble/_update_layer.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme/status_handling/_get_first_worst_error.py` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme/status_handling/_get_first_worst_error.py`

 * *Files identical despite different names*

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme.egg-info/PKG-INFO` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmed-kubeflow-chisme
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of helpers for Charms maintained by the Charmed Kubeflow team
 Home-page: https://github.com/canonical/charmed-kubeflow-chisme
 Author: Charmed Kubeflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -30,9 +30,14 @@
 
 [ckf]: https://charmed-kubeflow.io/
 [lightkube-rtd]: https://lightkube.readthedocs.io/en/latest/
 
 # Publishing to PyPi
 
 To publish a new release to Pypi:
-1. Update [setup.cfg](https://github.com/canonical/charmed-kubeflow-chisme/blob/main/setup.cfg#L3) to the new version and commit it to the repo via a completed PR
-2. Pull the repo and use `tox -e publish` to publish
+1. Update [setup.cfg](https://github.com/canonical/charmed-kubeflow-chisme/blob/main/setup.cfg#L3) to the new version 
+   and commit it to the repo via a completed PR
+2. Apply local git tag according to the format `X.X.X` (semantic versioning) on the main branch
+3. Push tag to the repo. Example: `git push origin 0.0.8`
+4. GitHub Action will create a new release on GitHub
+5. Edit release via GitHub UI and click publish
+6. GitHub Action will automatically publish the same commit to PyPi repository
```

### Comparing `charmed-kubeflow-chisme-0.0.8/src/charmed_kubeflow_chisme.egg-info/SOURCES.txt` & `charmed-kubeflow-chisme-0.0.9/src/charmed_kubeflow_chisme.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -27,12 +27,8 @@
 src/charmed_kubeflow_chisme/lightkube/batch/_sort_objects.py
 src/charmed_kubeflow_chisme/pebble/__init__.py
 src/charmed_kubeflow_chisme/pebble/_update_layer.py
 src/charmed_kubeflow_chisme/status_handling/__init__.py
 src/charmed_kubeflow_chisme/status_handling/_get_first_worst_error.py
 src/charmed_kubeflow_chisme/types/__init__.py
 src/charmed_kubeflow_chisme/types/_charm_status.py
-src/charmed_kubeflow_chisme/types/_lightkube.py
-tests/test_kubernetes.py
-tests/test_lightkube.py
-tests/test_pebble.py
-tests/test_status_handling.py
+src/charmed_kubeflow_chisme/types/_lightkube.py
```

