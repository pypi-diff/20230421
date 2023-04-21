# Comparing `tmp/google-cloud-gke-hub-1.8.1.tar.gz` & `tmp/google-cloud-gke-hub-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-gke-hub-1.8.1.tar", last modified: Mon Mar 27 14:52:12 2023, max compression
+gzip compressed data, was "google-cloud-gke-hub-1.9.0.tar", last modified: Wed Apr 19 23:24:34 2023, max compression
```

## Comparing `google-cloud-gke-hub-1.8.1.tar` & `google-cloud-gke-hub-1.9.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.534315 google-cloud-gke-hub-1.8.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4755 2023-03-27 14:52:12.534315 google-cloud-gke-hub-1.8.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3839 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.514315 google-cloud-gke-hub-1.8.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.514315 google-cloud-gke-hub-1.8.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.518315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub/
--rw-rw-r--   0 root         (0)     1003     2753 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.518315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/
--rw-rw-r--   0 root         (0)     1003     2597 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.518315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/
--rw-rw-r--   0 root         (0)     1003     1848 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      267 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       97 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.522315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.522315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/types/
--rw-rw-r--   0 root         (0)     1003     1729 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    24634 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/types/configmanagement.py
--rw-rw-r--   0 root         (0)     1003     4753 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.522315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/
--rw-rw-r--   0 root         (0)     1003      792 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      273 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003      100 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.522315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.522315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/types/
--rw-rw-r--   0 root         (0)     1003      673 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1351 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/types/multiclusteringress.py
--rw-rw-r--   0 root         (0)     1003       81 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.522315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.522315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/
--rw-rw-r--   0 root         (0)     1003      737 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/__init__.py
--rw-rw-r--   0 root         (0)     1003    63394 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/async_client.py
--rw-rw-r--   0 root         (0)     1003    74643 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/client.py
--rw-rw-r--   0 root         (0)     1003    10656 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.526315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/
--rw-rw-r--   0 root         (0)     1003     1288 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10633 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24498 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25045 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    63509 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.526315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/types/
--rw-rw-r--   0 root         (0)     1003     2359 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12050 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/types/feature.py
--rw-rw-r--   0 root         (0)     1003    18201 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/types/membership.py
--rw-rw-r--   0 root         (0)     1003    25881 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.526315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2500 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3880 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.526315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.526315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/
--rw-rw-r--   0 root         (0)     1003      805 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    72562 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    82543 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/client.py
--rw-rw-r--   0 root         (0)     1003     5829 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.530315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/
--rw-rw-r--   0 root         (0)     1003     1547 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12035 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    31588 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    32061 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    84492 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.530315 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2169 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    46501 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/types/membership.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.530315 google-cloud-gke-hub-1.8.1/google_cloud_gke_hub.egg-info/
--rw-r--r--   0 root         (0)     1003     4755 2023-03-27 14:52:12.000000 google-cloud-gke-hub-1.8.1/google_cloud_gke_hub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3615 2023-03-27 14:52:12.000000 google-cloud-gke-hub-1.8.1/google_cloud_gke_hub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:52:12.000000 google-cloud-gke-hub-1.8.1/google_cloud_gke_hub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:52:12.000000 google-cloud-gke-hub-1.8.1/google_cloud_gke_hub.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:52:12.000000 google-cloud-gke-hub-1.8.1/google_cloud_gke_hub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 14:52:12.000000 google-cloud-gke-hub-1.8.1/google_cloud_gke_hub.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:52:12.000000 google-cloud-gke-hub-1.8.1/google_cloud_gke_hub.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:52:12.534315 google-cloud-gke-hub-1.8.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3019 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.530315 google-cloud-gke-hub-1.8.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.530315 google-cloud-gke-hub-1.8.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.530315 google-cloud-gke-hub-1.8.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.530315 google-cloud-gke-hub-1.8.1/tests/unit/gapic/configmanagement_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/tests/unit/gapic/configmanagement_v1/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.530315 google-cloud-gke-hub-1.8.1/tests/unit/gapic/gkehub_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/tests/unit/gapic/gkehub_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   263635 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/tests/unit/gapic/gkehub_v1/test_gke_hub.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.534315 google-cloud-gke-hub-1.8.1/tests/unit/gapic/gkehub_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/tests/unit/gapic/gkehub_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   285312 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/tests/unit/gapic/gkehub_v1beta1/test_gke_hub_membership_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:12.534315 google-cloud-gke-hub-1.8.1/tests/unit/gapic/multiclusteringress_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:12.000000 google-cloud-gke-hub-1.8.1/tests/unit/gapic/multiclusteringress_v1/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.939446 google-cloud-gke-hub-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4755 2023-04-19 23:24:34.939446 google-cloud-gke-hub-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3839 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.923445 google-cloud-gke-hub-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.923445 google-cloud-gke-hub-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.927445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub/
+-rw-rw-r--   0 root         (0)     1003     2799 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.927445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/
+-rw-rw-r--   0 root         (0)     1003     2643 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.927445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/
+-rw-rw-r--   0 root         (0)     1003     1848 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      267 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       97 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.927445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.927445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1729 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24634 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/types/configmanagement.py
+-rw-rw-r--   0 root         (0)     1003     4753 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.927445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/
+-rw-rw-r--   0 root         (0)     1003      792 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      273 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003      100 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.927445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.927445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/types/
+-rw-rw-r--   0 root         (0)     1003      673 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1351 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/types/multiclusteringress.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.927445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.931445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/
+-rw-rw-r--   0 root         (0)     1003      737 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/__init__.py
+-rw-rw-r--   0 root         (0)     1003    63650 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/async_client.py
+-rw-rw-r--   0 root         (0)     1003    74899 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/client.py
+-rw-rw-r--   0 root         (0)     1003    10656 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.931445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/
+-rw-rw-r--   0 root         (0)     1003     1288 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10633 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24674 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25221 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    63685 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.931445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2405 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12050 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/types/feature.py
+-rw-rw-r--   0 root         (0)     1003    20923 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/types/membership.py
+-rw-rw-r--   0 root         (0)     1003    26263 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.931445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2500 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3880 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.931445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.935445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/
+-rw-rw-r--   0 root         (0)     1003      805 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    72562 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    82543 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5829 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.935445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1547 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12035 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    31588 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    32061 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    84492 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.935445 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2169 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46501 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/types/membership.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.935445 google-cloud-gke-hub-1.9.0/google_cloud_gke_hub.egg-info/
+-rw-r--r--   0 root         (0)     1003     4755 2023-04-19 23:24:34.000000 google-cloud-gke-hub-1.9.0/google_cloud_gke_hub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3615 2023-04-19 23:24:34.000000 google-cloud-gke-hub-1.9.0/google_cloud_gke_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-19 23:24:34.000000 google-cloud-gke-hub-1.9.0/google_cloud_gke_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-19 23:24:34.000000 google-cloud-gke-hub-1.9.0/google_cloud_gke_hub.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-19 23:24:34.000000 google-cloud-gke-hub-1.9.0/google_cloud_gke_hub.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-04-19 23:24:34.000000 google-cloud-gke-hub-1.9.0/google_cloud_gke_hub.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-19 23:24:34.000000 google-cloud-gke-hub-1.9.0/google_cloud_gke_hub.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-04-19 23:24:34.939446 google-cloud-gke-hub-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3019 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.935445 google-cloud-gke-hub-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.935445 google-cloud-gke-hub-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.935445 google-cloud-gke-hub-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.935445 google-cloud-gke-hub-1.9.0/tests/unit/gapic/configmanagement_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/tests/unit/gapic/configmanagement_v1/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.935445 google-cloud-gke-hub-1.9.0/tests/unit/gapic/gkehub_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/tests/unit/gapic/gkehub_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   265407 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/tests/unit/gapic/gkehub_v1/test_gke_hub.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.939446 google-cloud-gke-hub-1.9.0/tests/unit/gapic/gkehub_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/tests/unit/gapic/gkehub_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   285312 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/tests/unit/gapic/gkehub_v1beta1/test_gke_hub_membership_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-19 23:24:34.939446 google-cloud-gke-hub-1.9.0/tests/unit/gapic/multiclusteringress_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-19 23:22:44.000000 google-cloud-gke-hub-1.9.0/tests/unit/gapic/multiclusteringress_v1/__init__.py
```

### Comparing `google-cloud-gke-hub-1.8.1/LICENSE` & `google-cloud-gke-hub-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/MANIFEST.in` & `google-cloud-gke-hub-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/PKG-INFO` & `google-cloud-gke-hub-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-hub
-Version: 1.8.1
+Version: 1.9.0
 Summary: Google Cloud Gke Hub API client library
 Home-page: https://github.com/googleapis/python-gke-hub
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-gke-hub-1.8.1/README.rst` & `google-cloud-gke-hub-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     Authority,
     GkeCluster,
     KubernetesMetadata,
     KubernetesResource,
     Membership,
     MembershipEndpoint,
     MembershipState,
+    MonitoringConfig,
     ResourceManifest,
     ResourceOptions,
 )
 from google.cloud.gkehub_v1.types.service import (
     ConnectAgentResource,
     CreateFeatureRequest,
     CreateMembershipRequest,
@@ -73,14 +74,15 @@
     "Authority",
     "GkeCluster",
     "KubernetesMetadata",
     "KubernetesResource",
     "Membership",
     "MembershipEndpoint",
     "MembershipState",
+    "MonitoringConfig",
     "ResourceManifest",
     "ResourceOptions",
     "ConnectAgentResource",
     "CreateFeatureRequest",
     "CreateMembershipRequest",
     "DeleteFeatureRequest",
     "DeleteMembershipRequest",
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub/gapic_version.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     Authority,
     GkeCluster,
     KubernetesMetadata,
     KubernetesResource,
     Membership,
     MembershipEndpoint,
     MembershipState,
+    MonitoringConfig,
     ResourceManifest,
     ResourceOptions,
 )
 from .types.service import (
     ConnectAgentResource,
     CreateFeatureRequest,
     CreateMembershipRequest,
@@ -85,14 +86,15 @@
     "ListMembershipsRequest",
     "ListMembershipsResponse",
     "Membership",
     "MembershipEndpoint",
     "MembershipFeatureSpec",
     "MembershipFeatureState",
     "MembershipState",
+    "MonitoringConfig",
     "OperationMetadata",
     "ResourceManifest",
     "ResourceOptions",
     "TypeMeta",
     "UpdateFeatureRequest",
     "UpdateMembershipRequest",
 )
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/gapic_version.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/services/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/types/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/configmanagement_v1/types/configmanagement.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/configmanagement_v1/types/configmanagement.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/gapic_metadata.json` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/gapic_version.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/gapic_version.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/services/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/types/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/multiclusteringress_v1/types/multiclusteringress.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/multiclusteringress_v1/types/multiclusteringress.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/async_client.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,18 @@
     features over those clusters.
 
     The GKE Hub service operates on the following resources:
 
     -  [Membership][google.cloud.gkehub.v1.Membership]
     -  [Feature][google.cloud.gkehub.v1.Feature]
 
-    GKE Hub is currently only available in the global region.
+    GKE Hub is currently available in the global region and all regions
+    in https://cloud.google.com/compute/docs/regions-zones. Feature is
+    only available in global region while membership is global region
+    and all the regions.
 
     **Membership management may be non-trivial:** it is recommended to
     use one of the Google-provided client libraries or tools where
     possible when working with Membership resources.
     """
 
     _client: GkeHubClient
@@ -266,15 +269,16 @@
 
         Args:
             request (Optional[Union[google.cloud.gkehub_v1.types.ListMembershipsRequest, dict]]):
                 The request object. Request message for ``GkeHub.ListMemberships`` method.
             parent (:class:`str`):
                 Required. The parent (project and location) where the
                 Memberships will be listed. Specified in the format
-                ``projects/*/locations/*``.
+                ``projects/*/locations/*``. ``projects/*/locations/-``
+                list memberships in all the regions.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/client.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,18 @@
     features over those clusters.
 
     The GKE Hub service operates on the following resources:
 
     -  [Membership][google.cloud.gkehub.v1.Membership]
     -  [Feature][google.cloud.gkehub.v1.Feature]
 
-    GKE Hub is currently only available in the global region.
+    GKE Hub is currently available in the global region and all regions
+    in https://cloud.google.com/compute/docs/regions-zones. Feature is
+    only available in global region while membership is global region
+    and all the regions.
 
     **Membership management may be non-trivial:** it is recommended to
     use one of the Google-provided client libraries or tools where
     possible when working with Membership resources.
     """
 
     @staticmethod
@@ -525,15 +528,16 @@
 
         Args:
             request (Union[google.cloud.gkehub_v1.types.ListMembershipsRequest, dict]):
                 The request object. Request message for ``GkeHub.ListMemberships`` method.
             parent (str):
                 Required. The parent (project and location) where the
                 Memberships will be listed. Specified in the format
-                ``projects/*/locations/*``.
+                ``projects/*/locations/*``. ``projects/*/locations/-``
+                list memberships in all the regions.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/pagers.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/base.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/grpc.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,18 @@
     features over those clusters.
 
     The GKE Hub service operates on the following resources:
 
     -  [Membership][google.cloud.gkehub.v1.Membership]
     -  [Feature][google.cloud.gkehub.v1.Feature]
 
-    GKE Hub is currently only available in the global region.
+    GKE Hub is currently available in the global region and all regions
+    in https://cloud.google.com/compute/docs/regions-zones. Feature is
+    only available in global region while membership is global region
+    and all the regions.
 
     **Membership management may be non-trivial:** it is recommended to
     use one of the Google-provided client libraries or tools where
     possible when working with Membership resources.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/grpc_asyncio.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,18 @@
     features over those clusters.
 
     The GKE Hub service operates on the following resources:
 
     -  [Membership][google.cloud.gkehub.v1.Membership]
     -  [Feature][google.cloud.gkehub.v1.Feature]
 
-    GKE Hub is currently only available in the global region.
+    GKE Hub is currently available in the global region and all regions
+    in https://cloud.google.com/compute/docs/regions-zones. Feature is
+    only available in global region while membership is global region
+    and all the regions.
 
     **Membership management may be non-trivial:** it is recommended to
     use one of the Google-provided client libraries or tools where
     possible when working with Membership resources.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/services/gke_hub/transports/rest.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/services/gke_hub/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,18 @@
     features over those clusters.
 
     The GKE Hub service operates on the following resources:
 
     -  [Membership][google.cloud.gkehub.v1.Membership]
     -  [Feature][google.cloud.gkehub.v1.Feature]
 
-    GKE Hub is currently only available in the global region.
+    GKE Hub is currently available in the global region and all regions
+    in https://cloud.google.com/compute/docs/regions-zones. Feature is
+    only available in global region while membership is global region
+    and all the regions.
 
     **Membership management may be non-trivial:** it is recommended to
     use one of the Google-provided client libraries or tools where
     possible when working with Membership resources.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/types/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     Authority,
     GkeCluster,
     KubernetesMetadata,
     KubernetesResource,
     Membership,
     MembershipEndpoint,
     MembershipState,
+    MonitoringConfig,
     ResourceManifest,
     ResourceOptions,
 )
 from .service import (
     ConnectAgentResource,
     CreateFeatureRequest,
     CreateMembershipRequest,
@@ -64,14 +65,15 @@
     "Authority",
     "GkeCluster",
     "KubernetesMetadata",
     "KubernetesResource",
     "Membership",
     "MembershipEndpoint",
     "MembershipState",
+    "MonitoringConfig",
     "ResourceManifest",
     "ResourceOptions",
     "ConnectAgentResource",
     "CreateFeatureRequest",
     "CreateMembershipRequest",
     "DeleteFeatureRequest",
     "DeleteMembershipRequest",
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/types/feature.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/types/feature.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/types/membership.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/types/membership.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         "Membership",
         "MembershipEndpoint",
         "KubernetesResource",
         "ResourceOptions",
         "ResourceManifest",
         "GkeCluster",
         "KubernetesMetadata",
+        "MonitoringConfig",
         "MembershipState",
         "Authority",
     },
 )
 
 
 class Membership(proto.Message):
@@ -61,15 +62,15 @@
                ``-``
             3. It must start and end with an alphanumeric character
 
             Which can be expressed as the regex:
             ``[a-z0-9]([-a-z0-9]*[a-z0-9])?``, with a maximum length of
             63 characters.
         labels (MutableMapping[str, str]):
-            Optional. GCP labels for this membership.
+            Optional. Labels for this membership.
         description (str):
             Output only. Description of this membership, limited to 63
             characters. Must match the regex:
             ``[a-zA-Z0-9][a-zA-Z0-9_\-\.\ ]*``
 
             This field is present for legacy purposes.
         state (google.cloud.gkehub_v1.types.MembershipState):
@@ -107,14 +108,17 @@
             resource is deleted and another resource with the same name
             is created, it gets a different unique_id.
         authority (google.cloud.gkehub_v1.types.Authority):
             Optional. How to identify workloads from this
             Membership. See the documentation on Workload
             Identity for more details:
             https://cloud.google.com/kubernetes-engine/docs/how-to/workload-identity
+        monitoring_config (google.cloud.gkehub_v1.types.MonitoringConfig):
+            Optional. The monitoring config information
+            for this membership.
     """
 
     endpoint: "MembershipEndpoint" = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="type",
         message="MembershipEndpoint",
@@ -166,14 +170,19 @@
         number=11,
     )
     authority: "Authority" = proto.Field(
         proto.MESSAGE,
         number=12,
         message="Authority",
     )
+    monitoring_config: "MonitoringConfig" = proto.Field(
+        proto.MESSAGE,
+        number=14,
+        message="MonitoringConfig",
+    )
 
 
 class MembershipEndpoint(proto.Message):
     r"""MembershipEndpoint contains information needed to contact a
     Kubernetes API, endpoint and any additional Kubernetes metadata.
 
     Attributes:
@@ -190,14 +199,18 @@
 
             -  Ensure that the cluster is exclusively registered to one
                and only one Hub Membership.
             -  Propagate Workload Pool Information available in the
                Membership Authority field.
             -  Ensure proper initial configuration of default Hub
                Features.
+        google_managed (bool):
+            Output only. Whether the lifecycle of this
+            membership is managed by a google cluster
+            platform service.
     """
 
     gke_cluster: "GkeCluster" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="GkeCluster",
     )
@@ -207,14 +220,18 @@
         message="KubernetesMetadata",
     )
     kubernetes_resource: "KubernetesResource" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="KubernetesResource",
     )
+    google_managed: bool = proto.Field(
+        proto.BOOL,
+        number=8,
+    )
 
 
 class KubernetesResource(proto.Message):
     r"""KubernetesResource contains the YAML manifests and
     configuration for Membership Kubernetes resources in the
     cluster. After CreateMembership or UpdateMembership, these
     resources should be re-applied in the cluster.
@@ -342,24 +359,32 @@
 
 
 class GkeCluster(proto.Message):
     r"""GkeCluster contains information specific to GKE clusters.
 
     Attributes:
         resource_link (str):
-            Immutable. Self-link of the GCP resource for
-            the GKE cluster. For example:
+            Immutable. Self-link of the Google Cloud
+            resource for the GKE cluster. For example:
+
             //container.googleapis.com/projects/my-project/locations/us-west1-a/clusters/my-cluster
             Zonal clusters are also supported.
+        cluster_missing (bool):
+            Output only. If cluster_missing is set then it denotes that
+            the GKE cluster no longer exists in the GKE Control Plane.
     """
 
     resource_link: str = proto.Field(
         proto.STRING,
         number=1,
     )
+    cluster_missing: bool = proto.Field(
+        proto.BOOL,
+        number=2,
+    )
 
 
 class KubernetesMetadata(proto.Message):
     r"""KubernetesMetadata provides informational metadata for
     Memberships representing Kubernetes clusters.
 
     Attributes:
@@ -412,14 +437,68 @@
     update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=100,
         message=timestamp_pb2.Timestamp,
     )
 
 
+class MonitoringConfig(proto.Message):
+    r"""This field informs Fleet-based applications/services/UIs with
+    the necessary information for where each underlying Cluster
+    reports its metrics.
+
+    Attributes:
+        project_id (str):
+            Immutable. Project used to report Metrics
+        location (str):
+            Immutable. Location used to report Metrics
+        cluster (str):
+            Immutable. Cluster name used to report metrics. For Anthos
+            on VMWare/Baremetal, it would be in format
+            ``memberClusters/cluster_name``; And for Anthos on
+            MultiCloud, it would be in format
+            ``{azureClusters, awsClusters}/cluster_name``.
+        kubernetes_metrics_prefix (str):
+            Kubernetes system metrics, if available, are
+            written to this prefix. This defaults to
+            kubernetes.io for GKE, and kubernetes.io/anthos
+            for Anthos eventually. Noted: Anthos MultiCloud
+            will have kubernetes.io prefix today but will
+            migration to be under kubernetes.io/anthos
+        cluster_hash (str):
+            Immutable. Cluster hash, this is a unique
+            string generated by google code, which does not
+            contain any PII, which we can use to reference
+            the cluster. This is expected to be created by
+            the monitoring stack and persisted into the
+            Cluster object as well as to GKE-Hub.
+    """
+
+    project_id: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    location: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    cluster: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    kubernetes_metrics_prefix: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    cluster_hash: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+
+
 class MembershipState(proto.Message):
     r"""MembershipState describes the state of a Membership resource.
 
     Attributes:
         code (google.cloud.gkehub_v1.types.MembershipState.Code):
             Output only. The current state of the
             Membership resource.
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1/types/service.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1/types/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 class ListMembershipsRequest(proto.Message):
     r"""Request message for ``GkeHub.ListMemberships`` method.
 
     Attributes:
         parent (str):
             Required. The parent (project and location) where the
             Memberships will be listed. Specified in the format
-            ``projects/*/locations/*``.
+            ``projects/*/locations/*``. ``projects/*/locations/-`` list
+            memberships in all the regions.
         page_size (int):
             Optional. When requesting a 'page' of resources,
             ``page_size`` specifies number of resources to return. If
             unspecified or set to 0, all resources will be returned.
         page_token (str):
             Optional. Token returned by previous call to
             ``ListMemberships`` which specifies the position in the list
@@ -248,24 +249,33 @@
             with the same request ID was received, and if
             so, will ignore the second request. This
             prevents clients from accidentally creating
             duplicate commitments.
             The request ID must be a valid UUID with the
             exception that zero UUID is not supported
             (00000000-0000-0000-0000-000000000000).
+        force (bool):
+            Optional. If set to true, any subresource
+            from this Membership will also be deleted.
+            Otherwise, the request will only work if the
+            Membership has no subresource.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     request_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
+    force: bool = proto.Field(
+        proto.BOOL,
+        number=3,
+    )
 
 
 class UpdateMembershipRequest(proto.Message):
     r"""Request message for ``GkeHub.UpdateMembership`` method.
 
     Attributes:
         name (str):
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/gapic_metadata.json` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/gapic_version.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.1"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/async_client.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/client.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/pagers.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/base.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/grpc.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/grpc_asyncio.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/rest.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/services/gke_hub_membership_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/types/__init__.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google/cloud/gkehub_v1beta1/types/membership.py` & `google-cloud-gke-hub-1.9.0/google/cloud/gkehub_v1beta1/types/membership.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/google_cloud_gke_hub.egg-info/PKG-INFO` & `google-cloud-gke-hub-1.9.0/google_cloud_gke_hub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-hub
-Version: 1.8.1
+Version: 1.9.0
 Summary: Google Cloud Gke Hub API client library
 Home-page: https://github.com/googleapis/python-gke-hub
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-gke-hub-1.8.1/google_cloud_gke_hub.egg-info/SOURCES.txt` & `google-cloud-gke-hub-1.9.0/google_cloud_gke_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/setup.py` & `google-cloud-gke-hub-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/tests/__init__.py` & `google-cloud-gke-hub-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/tests/unit/__init__.py` & `google-cloud-gke-hub-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/tests/unit/gapic/__init__.py` & `google-cloud-gke-hub-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/tests/unit/gapic/configmanagement_v1/__init__.py` & `google-cloud-gke-hub-1.9.0/tests/unit/gapic/configmanagement_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/tests/unit/gapic/gkehub_v1/__init__.py` & `google-cloud-gke-hub-1.9.0/tests/unit/gapic/gkehub_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/tests/unit/gapic/gkehub_v1/test_gke_hub.py` & `google-cloud-gke-hub-1.9.0/tests/unit/gapic/gkehub_v1/test_gke_hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -4721,15 +4721,18 @@
         transport="rest",
     )
 
     # send a request that will satisfy transcoding
     request_init = {"parent": "projects/sample1/locations/sample2"}
     request_init["resource"] = {
         "endpoint": {
-            "gke_cluster": {"resource_link": "resource_link_value"},
+            "gke_cluster": {
+                "resource_link": "resource_link_value",
+                "cluster_missing": True,
+            },
             "kubernetes_metadata": {
                 "kubernetes_api_server_version": "kubernetes_api_server_version_value",
                 "node_provider_id": "node_provider_id_value",
                 "node_count": 1070,
                 "vcpu_count": 1094,
                 "memory_mb": 967,
                 "update_time": {"seconds": 751, "nanos": 543},
@@ -4742,14 +4745,15 @@
                 "connect_resources": {},
                 "resource_options": {
                     "connect_version": "connect_version_value",
                     "v1beta1_crd": True,
                     "k8s_version": "k8s_version_value",
                 },
             },
+            "google_managed": True,
         },
         "name": "name_value",
         "labels": {},
         "description": "description_value",
         "state": {"code": 1},
         "create_time": {},
         "update_time": {},
@@ -4759,14 +4763,21 @@
         "unique_id": "unique_id_value",
         "authority": {
             "issuer": "issuer_value",
             "workload_identity_pool": "workload_identity_pool_value",
             "identity_provider": "identity_provider_value",
             "oidc_jwks": b"oidc_jwks_blob",
         },
+        "monitoring_config": {
+            "project_id": "project_id_value",
+            "location": "location_value",
+            "cluster": "cluster_value",
+            "kubernetes_metrics_prefix": "kubernetes_metrics_prefix_value",
+            "cluster_hash": "cluster_hash_value",
+        },
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -4968,15 +4979,18 @@
         transport=transport,
     )
 
     # send a request that will satisfy transcoding
     request_init = {"parent": "projects/sample1/locations/sample2"}
     request_init["resource"] = {
         "endpoint": {
-            "gke_cluster": {"resource_link": "resource_link_value"},
+            "gke_cluster": {
+                "resource_link": "resource_link_value",
+                "cluster_missing": True,
+            },
             "kubernetes_metadata": {
                 "kubernetes_api_server_version": "kubernetes_api_server_version_value",
                 "node_provider_id": "node_provider_id_value",
                 "node_count": 1070,
                 "vcpu_count": 1094,
                 "memory_mb": 967,
                 "update_time": {"seconds": 751, "nanos": 543},
@@ -4989,14 +5003,15 @@
                 "connect_resources": {},
                 "resource_options": {
                     "connect_version": "connect_version_value",
                     "v1beta1_crd": True,
                     "k8s_version": "k8s_version_value",
                 },
             },
+            "google_managed": True,
         },
         "name": "name_value",
         "labels": {},
         "description": "description_value",
         "state": {"code": 1},
         "create_time": {},
         "update_time": {},
@@ -5006,14 +5021,21 @@
         "unique_id": "unique_id_value",
         "authority": {
             "issuer": "issuer_value",
             "workload_identity_pool": "workload_identity_pool_value",
             "identity_provider": "identity_provider_value",
             "oidc_jwks": b"oidc_jwks_blob",
         },
+        "monitoring_config": {
+            "project_id": "project_id_value",
+            "location": "location_value",
+            "cluster": "cluster_value",
+            "kubernetes_metrics_prefix": "kubernetes_metrics_prefix_value",
+            "cluster_hash": "cluster_hash_value",
+        },
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -5383,15 +5405,20 @@
 
     jsonified_request["name"] = "name_value"
 
     unset_fields = transport_class(
         credentials=ga_credentials.AnonymousCredentials()
     ).delete_membership._get_unset_required_fields(jsonified_request)
     # Check that path parameters and body parameters are not mixing in.
-    assert not set(unset_fields) - set(("request_id",))
+    assert not set(unset_fields) - set(
+        (
+            "force",
+            "request_id",
+        )
+    )
     jsonified_request.update(unset_fields)
 
     # verify required fields with non-default values are left alone
     assert "name" in jsonified_request
     assert jsonified_request["name"] == "name_value"
 
     client = GkeHubClient(
@@ -5434,15 +5461,23 @@
 
 def test_delete_membership_rest_unset_required_fields():
     transport = transports.GkeHubRestTransport(
         credentials=ga_credentials.AnonymousCredentials
     )
 
     unset_fields = transport.delete_membership._get_unset_required_fields({})
-    assert set(unset_fields) == (set(("requestId",)) & set(("name",)))
+    assert set(unset_fields) == (
+        set(
+            (
+                "force",
+                "requestId",
+            )
+        )
+        & set(("name",))
+    )
 
 
 @pytest.mark.parametrize("null_interceptor", [True, False])
 def test_delete_membership_rest_interceptors(null_interceptor):
     transport = transports.GkeHubRestTransport(
         credentials=ga_credentials.AnonymousCredentials(),
         interceptor=None if null_interceptor else transports.GkeHubRestInterceptor(),
@@ -5772,15 +5807,18 @@
         transport="rest",
     )
 
     # send a request that will satisfy transcoding
     request_init = {"name": "projects/sample1/locations/sample2/memberships/sample3"}
     request_init["resource"] = {
         "endpoint": {
-            "gke_cluster": {"resource_link": "resource_link_value"},
+            "gke_cluster": {
+                "resource_link": "resource_link_value",
+                "cluster_missing": True,
+            },
             "kubernetes_metadata": {
                 "kubernetes_api_server_version": "kubernetes_api_server_version_value",
                 "node_provider_id": "node_provider_id_value",
                 "node_count": 1070,
                 "vcpu_count": 1094,
                 "memory_mb": 967,
                 "update_time": {"seconds": 751, "nanos": 543},
@@ -5793,14 +5831,15 @@
                 "connect_resources": {},
                 "resource_options": {
                     "connect_version": "connect_version_value",
                     "v1beta1_crd": True,
                     "k8s_version": "k8s_version_value",
                 },
             },
+            "google_managed": True,
         },
         "name": "name_value",
         "labels": {},
         "description": "description_value",
         "state": {"code": 1},
         "create_time": {},
         "update_time": {},
@@ -5810,14 +5849,21 @@
         "unique_id": "unique_id_value",
         "authority": {
             "issuer": "issuer_value",
             "workload_identity_pool": "workload_identity_pool_value",
             "identity_provider": "identity_provider_value",
             "oidc_jwks": b"oidc_jwks_blob",
         },
+        "monitoring_config": {
+            "project_id": "project_id_value",
+            "location": "location_value",
+            "cluster": "cluster_value",
+            "kubernetes_metrics_prefix": "kubernetes_metrics_prefix_value",
+            "cluster_hash": "cluster_hash_value",
+        },
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -6006,15 +6052,18 @@
         transport=transport,
     )
 
     # send a request that will satisfy transcoding
     request_init = {"name": "projects/sample1/locations/sample2/memberships/sample3"}
     request_init["resource"] = {
         "endpoint": {
-            "gke_cluster": {"resource_link": "resource_link_value"},
+            "gke_cluster": {
+                "resource_link": "resource_link_value",
+                "cluster_missing": True,
+            },
             "kubernetes_metadata": {
                 "kubernetes_api_server_version": "kubernetes_api_server_version_value",
                 "node_provider_id": "node_provider_id_value",
                 "node_count": 1070,
                 "vcpu_count": 1094,
                 "memory_mb": 967,
                 "update_time": {"seconds": 751, "nanos": 543},
@@ -6027,14 +6076,15 @@
                 "connect_resources": {},
                 "resource_options": {
                     "connect_version": "connect_version_value",
                     "v1beta1_crd": True,
                     "k8s_version": "k8s_version_value",
                 },
             },
+            "google_managed": True,
         },
         "name": "name_value",
         "labels": {},
         "description": "description_value",
         "state": {"code": 1},
         "create_time": {},
         "update_time": {},
@@ -6044,14 +6094,21 @@
         "unique_id": "unique_id_value",
         "authority": {
             "issuer": "issuer_value",
             "workload_identity_pool": "workload_identity_pool_value",
             "identity_provider": "identity_provider_value",
             "oidc_jwks": b"oidc_jwks_blob",
         },
+        "monitoring_config": {
+            "project_id": "project_id_value",
+            "location": "location_value",
+            "cluster": "cluster_value",
+            "kubernetes_metrics_prefix": "kubernetes_metrics_prefix_value",
+            "cluster_hash": "cluster_hash_value",
+        },
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
```

### Comparing `google-cloud-gke-hub-1.8.1/tests/unit/gapic/gkehub_v1beta1/__init__.py` & `google-cloud-gke-hub-1.9.0/tests/unit/gapic/gkehub_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/tests/unit/gapic/gkehub_v1beta1/test_gke_hub_membership_service.py` & `google-cloud-gke-hub-1.9.0/tests/unit/gapic/gkehub_v1beta1/test_gke_hub_membership_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-hub-1.8.1/tests/unit/gapic/multiclusteringress_v1/__init__.py` & `google-cloud-gke-hub-1.9.0/tests/unit/gapic/multiclusteringress_v1/__init__.py`

 * *Files identical despite different names*

