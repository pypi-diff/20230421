# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-6.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-6.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-cncf-kubernetes-6.0.0rc1.tar", last modified: Sun Apr  9 13:48:22 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-cncf-kubernetes-6.1.0rc1.tar", last modified: Fri Apr 21 19:48:12 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1.tar` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1156 2023-04-09 13:48:20.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    32291 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    30737 2023-04-09 13:48:20.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6151 2023-03-16 20:46:35.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     4323 2023-04-09 13:48:20.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23857 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    37598 2023-04-08 17:35:35.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-03-15 08:58:48.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3343 2023-03-27 08:32:49.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1072 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    10454 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21693 2023-04-08 17:35:35.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)    32291 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 13:48:21.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1976 2023-04-09 13:48:22.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-04-09 13:48:19.000000 apache-airflow-providers-cncf-kubernetes-6.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-04-21 19:48:10.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    32810 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    31256 2023-04-21 19:48:10.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6151 2023-03-16 20:46:35.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-04-21 19:48:10.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23857 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    39116 2023-04-21 18:38:06.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2023-03-15 08:58:48.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3343 2023-03-27 08:32:49.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    10454 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21693 2023-04-13 08:25:20.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    32810 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-04-21 19:48:10.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/LICENSE` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 6.0.0rc1
+Version: 6.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``6.0.0rc1``
+Release: ``6.1.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -112,14 +112,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.0
+.....
+
+Features
+~~~~~~~~
+
+* ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
+* ``Skip KubernetesPodOperator task when it returns a provided exit code (#29000)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Deprecate 'skip_exit_code' in 'DockerOperator' and 'KubernetesPodOperator' (#30733)``
+  * ``Remove skip_exit_code from KubernetesPodOperator (#30788)``
+
 6.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 Use ``kubernetes_default`` connection by default in the ``KubernetesPodOperator``.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/README.rst` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``6.0.0rc1``
+Release: ``6.1.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,14 +79,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.0
+.....
+
+Features
+~~~~~~~~
+
+* ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
+* ``Skip KubernetesPodOperator task when it returns a provided exit code (#29000)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Deprecate 'skip_exit_code' in 'DockerOperator' and 'KubernetesPodOperator' (#30733)``
+  * ``Remove skip_exit_code from KubernetesPodOperator (#30788)``
+
 6.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 Use ``kubernetes_default`` connection by default in the ``KubernetesPodOperator``.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cncf-kubernetes",
         "name": "Kubernetes",
         "description": "`Kubernetes <https://kubernetes.io/>`__\n",
         "suspended": False,
         "versions": [
+            "6.1.0",
             "6.0.0",
             "5.3.0",
             "5.2.2",
             "5.2.1",
             "5.2.0",
             "5.1.1",
             "5.1.0",
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,23 +21,24 @@
 import json
 import logging
 import os
 import re
 import secrets
 import string
 import warnings
+from collections.abc import Container
 from contextlib import AbstractContextManager
 from typing import TYPE_CHECKING, Any, Sequence
 
 from kubernetes.client import CoreV1Api, models as k8s
 from slugify import slugify
 from urllib3.exceptions import HTTPError
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowSkipException
 from airflow.kubernetes import pod_generator
 from airflow.kubernetes.pod_generator import PodGenerator
 from airflow.kubernetes.secret import Secret
 from airflow.models import BaseOperator
 from airflow.providers.cncf.kubernetes.backcompat.backwards_compat_converters import (
     convert_affinity,
     convert_configmap,
@@ -209,14 +210,17 @@
         to be set in the container.
     :param termination_grace_period: Termination grace period if task killed in UI,
         defaults to kubernetes default
     :param configmaps: (Optional) A list of names of config maps from which it collects ConfigMaps
         to populate the environment variables with. The contents of the target
         ConfigMap's Data field will represent the key-value pairs as environment variables.
         Extends env_from.
+    :param skip_on_exit_code: If task exits with this exit code, leave the task
+        in ``skipped`` state (default: None). If set to ``None``, any non-zero
+        exit code will be treated as a failure.
     :param base_container_name: The name of the base container in the pod. This container's logs
         will appear as part of this task's logs if get_logs is True. Defaults to None. If None,
         will consult the class variable BASE_CONTAINER_NAME (which defaults to "base") for the base
         container name to use.
     :param deferrable: Run operator in the deferrable mode.
     :param poll_interval: Polling period in seconds to check for the status. Used only in deferrable mode.
     """
@@ -284,14 +288,15 @@
         log_events_on_failure: bool = False,
         do_xcom_push: bool = False,
         pod_template_file: str | None = None,
         priority_class_name: str | None = None,
         pod_runtime_info_envs: list[k8s.V1EnvVar] | None = None,
         termination_grace_period: int | None = None,
         configmaps: list[str] | None = None,
+        skip_on_exit_code: int | Container[int] | None = None,
         base_container_name: str | None = None,
         deferrable: bool = False,
         poll_interval: float = 2,
         **kwargs,
     ) -> None:
         # TODO: remove in provider 6.0.0 release. This is a mitigate step to advise users to switch to the
         # container_resources parameter.
@@ -353,14 +358,21 @@
         self.priority_class_name = priority_class_name
         self.pod_template_file = pod_template_file
         self.name = self._set_name(name)
         self.random_name_suffix = random_name_suffix
         self.termination_grace_period = termination_grace_period
         self.pod_request_obj: k8s.V1Pod | None = None
         self.pod: k8s.V1Pod | None = None
+        self.skip_on_exit_code = (
+            skip_on_exit_code
+            if isinstance(skip_on_exit_code, Container)
+            else [skip_on_exit_code]
+            if skip_on_exit_code
+            else []
+        )
         self.base_container_name = base_container_name or self.BASE_CONTAINER_NAME
         self.deferrable = deferrable
         self.poll_interval = poll_interval
         self.remote_pod: k8s.V1Pod | None = None
 
         self._config_dict: dict | None = None
 
@@ -666,14 +678,33 @@
             if self.log_events_on_failure:
                 self._read_pod_events(pod, reraise=False)
 
             self.process_pod_deletion(remote_pod, reraise=False)
 
             error_message = get_container_termination_message(remote_pod, self.base_container_name)
             error_message = "\n" + error_message if error_message else ""
+            if self.skip_on_exit_code is not None:
+                container_statuses = (
+                    remote_pod.status.container_statuses if remote_pod and remote_pod.status else None
+                ) or []
+                base_container_status = next(
+                    (x for x in container_statuses if x.name == self.base_container_name), None
+                )
+                exit_code = (
+                    base_container_status.last_state.terminated.exit_code
+                    if base_container_status
+                    and base_container_status.last_state
+                    and base_container_status.last_state.terminated
+                    else None
+                )
+                if exit_code in self.skip_on_exit_code:
+                    raise AirflowSkipException(
+                        f"Pod {pod and pod.metadata.name} returned exit code "
+                        f"{self.skip_on_exit_code}. Skipping."
+                    )
             raise AirflowException(
                 f"Pod {pod and pod.metadata.name} returned a failure:\n{error_message}\n"
                 f"remote_pod: {remote_pod}"
             )
         else:
             self.process_pod_deletion(remote_pod, reraise=False)
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 6.0.0rc1
+Version: 6.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``6.0.0rc1``
+Release: ``6.1.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -112,14 +112,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.0
+.....
+
+Features
+~~~~~~~~
+
+* ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
+* ``Skip KubernetesPodOperator task when it returns a provided exit code (#29000)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Deprecate 'skip_exit_code' in 'DockerOperator' and 'KubernetesPodOperator' (#30733)``
+  * ``Remove skip_exit_code from KubernetesPodOperator (#30788)``
+
 6.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 Use ``kubernetes_default`` connection by default in the ``KubernetesPodOperator``.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.0.0rc1/setup.py` & `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-cncf-kubernetes package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.0.0"
+version = "6.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-cncf-kubernetes setup."""
     setup(
         version=version,
         extras_require={},
```

