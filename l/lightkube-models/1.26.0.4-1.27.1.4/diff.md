# Comparing `tmp/lightkube-models-1.26.0.4.tar.gz` & `tmp/lightkube-models-1.27.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lightkube-models-1.26.0.4.tar", last modified: Thu Dec 22 11:59:23 2022, max compression
+gzip compressed data, was "dist/lightkube-models-1.27.1.4.tar", last modified: Fri Apr 21 16:02:28 2023, max compression
```

## Comparing `lightkube-models-1.26.0.4.tar` & `lightkube-models-1.27.1.4.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/
--rw-r--r--   0 tribulat   (501) staff       (20)     1096 2021-01-09 13:57:13.000000 lightkube-models-1.26.0.4/LICENSE
--rw-r--r--   0 tribulat   (501) staff       (20)     1225 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/PKG-INFO
--rw-r--r--   0 tribulat   (501) staff       (20)      417 2020-09-14 18:55:30.000000 lightkube-models-1.26.0.4/README.md
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/lightkube/
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/lightkube/models/
--rw-r--r--   0 tribulat   (501) staff       (20)       25 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/__init__.py
--rw-r--r--   0 tribulat   (501) staff       (20)    25010 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/admissionregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    21450 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/admissionregistration_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    37501 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/apiextensions_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     7990 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/apiregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     5593 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/apiserverinternal_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    47013 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/apps_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     8423 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/authentication_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2042 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/authentication_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    16556 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/authorization_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     8576 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/autoscaling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    26103 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/autoscaling_v2.py
--rw-r--r--   0 tribulat   (501) staff       (20)    26395 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/batch_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    13382 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/certificates_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     3765 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/coordination_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)   303235 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/core_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     9333 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/discovery_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     7116 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/events_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    25122 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/flowcontrol_v1beta2.py
--rw-r--r--   0 tribulat   (501) staff       (20)    25145 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/flowcontrol_v1beta3.py
--rw-r--r--   0 tribulat   (501) staff       (20)    38337 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/meta_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    31992 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/networking_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     4843 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/networking_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     5545 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/node_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    10374 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/policy_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    14684 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/rbac_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      164 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/resource.py
--rw-r--r--   0 tribulat   (501) staff       (20)    20692 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/resource_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      193 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/runtime.py
--rw-r--r--   0 tribulat   (501) staff       (20)     3809 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/scheduling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    34440 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/storage_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     6290 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/storage_v1beta1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      204 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/util_intstr.py
--rw-r--r--   0 tribulat   (501) staff       (20)      795 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/models/version.py
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/lightkube/resources/
--rw-r--r--   0 tribulat   (501) staff       (20)     1468 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/admissionregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1512 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/admissionregistration_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1504 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/apiextensions_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1340 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/apiregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     7160 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/apps_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      547 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/authentication_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      607 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/authentication_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1952 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/authorization_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1525 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/autoscaling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1525 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/autoscaling_v2.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2342 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/batch_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2249 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/certificates_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      716 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/coordination_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    17870 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/core_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      741 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/discovery_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      686 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/events_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2812 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/flowcontrol_apiserver_v1beta2.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2812 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/flowcontrol_apiserver_v1beta3.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1467 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/internal_apiserver_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     3133 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/networking_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      701 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/networking_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      647 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/node_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1428 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/policy_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2360 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/rbac_authorization_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     3944 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/resource_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      682 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/scheduling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     3503 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/storage_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      782 2022-12-22 11:59:18.000000 lightkube-models-1.26.0.4/lightkube/resources/storage_v1beta1.py
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/lightkube_models.egg-info/
--rw-r--r--   0 tribulat   (501) staff       (20)     1225 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/lightkube_models.egg-info/PKG-INFO
--rw-r--r--   0 tribulat   (501) staff       (20)     2493 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/lightkube_models.egg-info/SOURCES.txt
--rw-r--r--   0 tribulat   (501) staff       (20)        1 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/lightkube_models.egg-info/dependency_links.txt
--rw-r--r--   0 tribulat   (501) staff       (20)       10 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/lightkube_models.egg-info/top_level.txt
--rw-r--r--   0 tribulat   (501) staff       (20)       38 2022-12-22 11:59:23.000000 lightkube-models-1.26.0.4/setup.cfg
--rw-r--r--   0 tribulat   (501) staff       (20)      959 2021-01-09 13:57:13.000000 lightkube-models-1.26.0.4/setup.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2023-04-21 16:02:28.000000 lightkube-models-1.27.1.4/
+-rw-r--r--   0 tribulat   (501) staff       (20)     1096 2021-01-09 13:57:13.000000 lightkube-models-1.27.1.4/LICENSE
+-rw-r--r--   0 tribulat   (501) staff       (20)     1225 2023-04-21 16:02:28.000000 lightkube-models-1.27.1.4/PKG-INFO
+-rw-r--r--   0 tribulat   (501) staff       (20)      417 2020-09-14 18:55:30.000000 lightkube-models-1.27.1.4/README.md
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2023-04-21 16:02:27.000000 lightkube-models-1.27.1.4/lightkube/
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2023-04-21 16:02:28.000000 lightkube-models-1.27.1.4/lightkube/models/
+-rw-r--r--   0 tribulat   (501) staff       (20)       25 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/__init__.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    28953 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/admissionregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    33170 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/admissionregistration_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    38717 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/apiextensions_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     7990 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/apiregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5593 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/apiserverinternal_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    47228 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/apps_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     8423 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/authentication_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2185 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/authentication_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2185 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/authentication_v1beta1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    16556 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/authorization_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     8981 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/autoscaling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    26169 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/autoscaling_v2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    26394 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/batch_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    13382 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/certificates_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5314 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/certificates_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     3783 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/coordination_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)   307522 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/core_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     9923 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/discovery_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     7116 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/events_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    25122 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/flowcontrol_v1beta2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    25145 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/flowcontrol_v1beta3.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    38555 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/meta_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    32235 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/networking_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     9182 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/networking_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5545 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/node_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    10372 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/policy_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    14684 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/rbac_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      164 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/resource.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    22482 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/resource_v1alpha2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      193 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/runtime.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     3842 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/scheduling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    34830 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/storage_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      204 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/util_intstr.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      795 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/models/version.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2023-04-21 16:02:28.000000 lightkube-models-1.27.1.4/lightkube/resources/
+-rw-r--r--   0 tribulat   (501) staff       (20)     1468 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/admissionregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2330 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/admissionregistration_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1504 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/apiextensions_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1340 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/apiregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     7160 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/apps_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      547 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/authentication_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      607 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/authentication_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      602 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/authentication_v1beta1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1952 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/authorization_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1525 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/autoscaling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1525 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/autoscaling_v2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2342 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/batch_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2249 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/certificates_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      746 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/certificates_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      716 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/coordination_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    17870 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/core_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      741 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/discovery_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      686 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/events_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2812 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/flowcontrol_apiserver_v1beta2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2812 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/flowcontrol_apiserver_v1beta3.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1467 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/internal_apiserver_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     3133 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/networking_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1239 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/networking_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      647 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/node_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1428 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/policy_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2360 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/rbac_authorization_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     4035 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/resource_v1alpha2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      682 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/scheduling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     3503 2023-04-21 16:02:23.000000 lightkube-models-1.27.1.4/lightkube/resources/storage_v1.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2023-04-21 16:02:28.000000 lightkube-models-1.27.1.4/lightkube_models.egg-info/
+-rw-r--r--   0 tribulat   (501) staff       (20)     1225 2023-04-21 16:02:27.000000 lightkube-models-1.27.1.4/lightkube_models.egg-info/PKG-INFO
+-rw-r--r--   0 tribulat   (501) staff       (20)     2594 2023-04-21 16:02:27.000000 lightkube-models-1.27.1.4/lightkube_models.egg-info/SOURCES.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)        1 2023-04-21 16:02:27.000000 lightkube-models-1.27.1.4/lightkube_models.egg-info/dependency_links.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)       10 2023-04-21 16:02:27.000000 lightkube-models-1.27.1.4/lightkube_models.egg-info/top_level.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)       38 2023-04-21 16:02:28.000000 lightkube-models-1.27.1.4/setup.cfg
+-rw-r--r--   0 tribulat   (501) staff       (20)      959 2021-01-09 13:57:13.000000 lightkube-models-1.27.1.4/setup.py
```

### Comparing `lightkube-models-1.26.0.4/LICENSE` & `lightkube-models-1.27.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/PKG-INFO` & `lightkube-models-1.27.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightkube-models
-Version: 1.26.0.4
+Version: 1.27.1.4
 Summary: Models and Resources for lightkube module
 Home-page: https://github.com/gtsystem/lightkube-models
 Author: Giuseppe Tribulato
 Author-email: gtsystem@gmail.com
 License: Apache Software License
 Description: # lightkube-models
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/admissionregistration_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/admissionregistration_v1.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,50 @@
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
 from . import meta_v1
 
 
 @dataclass
+class MatchCondition(DataclassDictMixIn):
+    """MatchCondition represents a condition which must by fulfilled for a request to
+      be sent to a webhook.
+
+      **parameters**
+
+      * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. Must
+        evaluate to bool. CEL expressions have access to the contents of the
+        AdmissionRequest and Authorizer, organized into CEL variables:
+        'object' - The object from the incoming request. The value is null for DELETE
+        requests. 'oldObject' - The existing object. The value is null for CREATE
+        requests. 'request' - Attributes of the admission
+        request(/pkg/apis/admission/types.go#AdmissionRequest). 'authorizer' - A CEL
+        Authorizer. May be used to perform authorization checks for the principal
+        (user or service account) of the request.
+          See https://pkg.go.dev/k8s.io/apiserver/pkg/cel/library#Authz
+        'authorizer.requestResource' - A CEL ResourceCheck constructed from the
+        'authorizer' and configured with the
+          request resource.
+        Documentation on CEL: https://kubernetes.io/docs/reference/using-api/cel/
+        Required.
+      * **name** ``str`` - Name is an identifier for this match condition, used for strategic merging of
+        MatchConditions, as well as providing an identifier for logging purposes. A
+        good name should be descriptive of the associated expression. Name must be a
+        qualified name consisting of alphanumeric characters, '-', '_' or '.', and
+        must start and end with an alphanumeric character (e.g. 'MyName',  or
+        'my.name',  or '123-abc', regex used for validation is
+        '([A-Za-z0-9][-A-Za-z0-9_.]*)?[A-Za-z0-9]') with an optional DNS subdomain
+        prefix and '/' (e.g. 'example.com/MyName')
+        Required.
+    """
+    expression: 'str'
+    name: 'str'
+
+
+@dataclass
 class MutatingWebhook(DataclassDictMixIn):
     """MutatingWebhook describes an admission webhook and the resources and
       operations it applies to.
 
       **parameters**
 
       * **admissionReviewVersions** ``List[str]`` - AdmissionReviewVersions is an ordered list of preferred `AdmissionReview`
@@ -30,14 +66,28 @@
         Unknown). Webhooks with side effects MUST implement a reconciliation system,
         since a request may be rejected by a future step in the admission chain and
         the side effects therefore need to be undone. Requests with the dryRun
         attribute will be auto-rejected if they match a webhook with sideEffects ==
         Unknown or Some.
       * **failurePolicy** ``str`` - *(optional)* FailurePolicy defines how unrecognized errors from the admission endpoint are
         handled - allowed values are Ignore or Fail. Defaults to Fail.
+      * **matchConditions** ``List[MatchCondition]`` - *(optional)* MatchConditions is a list of conditions that must be met for a request to be
+        sent to this webhook. Match conditions filter requests that have already been
+        matched by the rules, namespaceSelector, and objectSelector. An empty list of
+        matchConditions matches all requests. There are a maximum of 64 match
+        conditions allowed.
+        The exact matching logic is (in order):
+          1. If ANY matchCondition evaluates to FALSE, the webhook is skipped.
+          2. If ALL matchConditions evaluate to TRUE, the webhook is called.
+          3. If any matchCondition evaluates to an error (but none are FALSE):
+             - If failurePolicy=Fail, reject the request
+             - If failurePolicy=Ignore, the error is ignored and the webhook is
+        skipped
+        This is an alpha feature and managed by the AdmissionWebhookMatchConditions
+        feature gate.
       * **matchPolicy** ``str`` - *(optional)* matchPolicy defines how the "rules" list is used to match incoming requests.
         Allowed values are "Exact" or "Equivalent".
         - Exact: match a request only if it exactly matches a specified rule. For
         example, if deployments can be modified via apps/v1, apps/v1beta1, and
         extensions/v1beta1, but "rules" only included `apiGroups:["apps"],
         apiVersions:["v1"], resources: ["deployments"]`, a request to apps/v1beta1 or
         extensions/v1beta1 would not be sent to the webhook.
@@ -122,14 +172,15 @@
         Default to 10 seconds.
     """
     admissionReviewVersions: 'List[str]'
     clientConfig: 'WebhookClientConfig'
     name: 'str'
     sideEffects: 'str'
     failurePolicy: 'str' = None
+    matchConditions: 'List[MatchCondition]' = None
     matchPolicy: 'str' = None
     namespaceSelector: 'meta_v1.LabelSelector' = None
     objectSelector: 'meta_v1.LabelSelector' = None
     reinvocationPolicy: 'str' = None
     rules: 'List[RuleWithOperations]' = None
     timeoutSeconds: 'int' = None
 
@@ -264,14 +315,28 @@
         Unknown). Webhooks with side effects MUST implement a reconciliation system,
         since a request may be rejected by a future step in the admission chain and
         the side effects therefore need to be undone. Requests with the dryRun
         attribute will be auto-rejected if they match a webhook with sideEffects ==
         Unknown or Some.
       * **failurePolicy** ``str`` - *(optional)* FailurePolicy defines how unrecognized errors from the admission endpoint are
         handled - allowed values are Ignore or Fail. Defaults to Fail.
+      * **matchConditions** ``List[MatchCondition]`` - *(optional)* MatchConditions is a list of conditions that must be met for a request to be
+        sent to this webhook. Match conditions filter requests that have already been
+        matched by the rules, namespaceSelector, and objectSelector. An empty list of
+        matchConditions matches all requests. There are a maximum of 64 match
+        conditions allowed.
+        The exact matching logic is (in order):
+          1. If ANY matchCondition evaluates to FALSE, the webhook is skipped.
+          2. If ALL matchConditions evaluate to TRUE, the webhook is called.
+          3. If any matchCondition evaluates to an error (but none are FALSE):
+             - If failurePolicy=Fail, reject the request
+             - If failurePolicy=Ignore, the error is ignored and the webhook is
+        skipped
+        This is an alpha feature and managed by the AdmissionWebhookMatchConditions
+        feature gate.
       * **matchPolicy** ``str`` - *(optional)* matchPolicy defines how the "rules" list is used to match incoming requests.
         Allowed values are "Exact" or "Equivalent".
         - Exact: match a request only if it exactly matches a specified rule. For
         example, if deployments can be modified via apps/v1, apps/v1beta1, and
         extensions/v1beta1, but "rules" only included `apiGroups:["apps"],
         apiVersions:["v1"], resources: ["deployments"]`, a request to apps/v1beta1 or
         extensions/v1beta1 would not be sent to the webhook.
@@ -340,14 +405,15 @@
         Default to 10 seconds.
     """
     admissionReviewVersions: 'List[str]'
     clientConfig: 'WebhookClientConfig'
     name: 'str'
     sideEffects: 'str'
     failurePolicy: 'str' = None
+    matchConditions: 'List[MatchCondition]' = None
     matchPolicy: 'str' = None
     namespaceSelector: 'meta_v1.LabelSelector' = None
     objectSelector: 'meta_v1.LabelSelector' = None
     rules: 'List[RuleWithOperations]' = None
     timeoutSeconds: 'int' = None
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/admissionregistration_v1alpha1.py` & `lightkube-models-1.27.1.4/lightkube/models/admissionregistration_v1alpha1.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,101 @@
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
 from . import meta_v1
 
 
 @dataclass
+class AuditAnnotation(DataclassDictMixIn):
+    """AuditAnnotation describes how to produce an audit annotation for an API
+      request.
+
+      **parameters**
+
+      * **key** ``str`` - key specifies the audit annotation key. The audit annotation keys of a
+        ValidatingAdmissionPolicy must be unique. The key must be a qualified name
+        ([A-Za-z0-9][-A-Za-z0-9_.]*) no more than 63 bytes in length.
+        The key is combined with the resource name of the ValidatingAdmissionPolicy to
+        construct an audit annotation key: "{ValidatingAdmissionPolicy name}/{key}".
+        If an admission webhook uses the same resource name as this
+        ValidatingAdmissionPolicy and the same audit annotation key, the annotation
+        key will be identical. In this case, the first annotation written with the key
+        will be included in the audit event and all subsequent annotations with the
+        same key will be discarded.
+        Required.
+      * **valueExpression** ``str`` - valueExpression represents the expression which is evaluated by CEL to produce
+        an audit annotation value. The expression must evaluate to either a string or
+        null value. If the expression evaluates to a string, the audit annotation is
+        included with the string value. If the expression evaluates to null or empty
+        string the audit annotation will be omitted. The valueExpression may be no
+        longer than 5kb in length. If the result of the valueExpression is more than
+        10kb in length, it will be truncated to 10kb.
+        If multiple ValidatingAdmissionPolicyBinding resources match an API request,
+        then the valueExpression will be evaluated for each binding. All unique values
+        produced by the valueExpressions will be joined together in a comma-separated
+        list.
+        Required.
+    """
+    key: 'str'
+    valueExpression: 'str'
+
+
+@dataclass
+class ExpressionWarning(DataclassDictMixIn):
+    """ExpressionWarning is a warning information that targets a specific expression.
+
+      **parameters**
+
+      * **fieldRef** ``str`` - The path to the field that refers the expression. For example, the reference
+        to the expression of the first item of validations is
+        "spec.validations[0].expression"
+      * **warning** ``str`` - The content of type checking information in a human-readable form. Each line
+        of the warning contains the type that the expression is checked against,
+        followed by the type check error from the compiler.
+    """
+    fieldRef: 'str'
+    warning: 'str'
+
+
+@dataclass
+class MatchCondition(DataclassDictMixIn):
+    """
+
+      **parameters**
+
+      * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. Must
+        evaluate to bool. CEL expressions have access to the contents of the
+        AdmissionRequest and Authorizer, organized into CEL variables:
+        'object' - The object from the incoming request. The value is null for DELETE
+        requests. 'oldObject' - The existing object. The value is null for CREATE
+        requests. 'request' - Attributes of the admission
+        request(/pkg/apis/admission/types.go#AdmissionRequest). 'authorizer' - A CEL
+        Authorizer. May be used to perform authorization checks for the principal
+        (user or service account) of the request.
+          See https://pkg.go.dev/k8s.io/apiserver/pkg/cel/library#Authz
+        'authorizer.requestResource' - A CEL ResourceCheck constructed from the
+        'authorizer' and configured with the
+          request resource.
+        Documentation on CEL: https://kubernetes.io/docs/reference/using-api/cel/
+        Required.
+      * **name** ``str`` - Name is an identifier for this match condition, used for strategic merging of
+        MatchConditions, as well as providing an identifier for logging purposes. A
+        good name should be descriptive of the associated expression. Name must be a
+        qualified name consisting of alphanumeric characters, '-', '_' or '.', and
+        must start and end with an alphanumeric character (e.g. 'MyName',  or
+        'my.name',  or '123-abc', regex used for validation is
+        '([A-Za-z0-9][-A-Za-z0-9_.]*)?[A-Za-z0-9]') with an optional DNS subdomain
+        prefix and '/' (e.g. 'example.com/MyName')
+        Required.
+    """
+    expression: 'str'
+    name: 'str'
+
+
+@dataclass
 class MatchResources(DataclassDictMixIn):
     """MatchResources decides whether to run the admission control policy on an
       object based on whether it meets the match criteria. The exclude rules take
       precedence over include rules (if a resource matches both, it is excluded)
 
       **parameters**
 
@@ -154,14 +241,26 @@
         resources
     """
     name: 'str' = None
     namespace: 'str' = None
 
 
 @dataclass
+class TypeChecking(DataclassDictMixIn):
+    """TypeChecking contains results of type checking the expressions in the
+      ValidatingAdmissionPolicy
+
+      **parameters**
+
+      * **expressionWarnings** ``List[ExpressionWarning]`` - *(optional)* The type checking warnings for each expression.
+    """
+    expressionWarnings: 'List[ExpressionWarning]' = None
+
+
+@dataclass
 class ValidatingAdmissionPolicy(DataclassDictMixIn):
     """ValidatingAdmissionPolicy describes the definition of an admission validation
       policy that accepts or rejects an object without changing it.
 
       **parameters**
 
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
@@ -171,19 +270,23 @@
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object metadata; More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.
       * **spec** ``ValidatingAdmissionPolicySpec`` - *(optional)* Specification of the desired behavior of the ValidatingAdmissionPolicy.
+      * **status** ``ValidatingAdmissionPolicyStatus`` - *(optional)* The status of the ValidatingAdmissionPolicy, including warnings that are
+        useful to determine if the policy behaves in the expected way. Populated by
+        the system. Read-only.
     """
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
     spec: 'ValidatingAdmissionPolicySpec' = None
+    status: 'ValidatingAdmissionPolicyStatus' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyBinding(DataclassDictMixIn):
     """ValidatingAdmissionPolicyBinding binds the ValidatingAdmissionPolicy with
       paramerized resources. ValidatingAdmissionPolicyBinding and parameter CRDs
       together define how cluster administrators configure policies for clusters.
@@ -253,18 +356,53 @@
         ParamKind of the bound ValidatingAdmissionPolicy. If the policy specifies a
         ParamKind and the resource referred to by ParamRef does not exist, this
         binding is considered mis-configured and the FailurePolicy of the
         ValidatingAdmissionPolicy applied.
       * **policyName** ``str`` - *(optional)* PolicyName references a ValidatingAdmissionPolicy name which the
         ValidatingAdmissionPolicyBinding binds to. If the referenced resource does not
         exist, this binding is considered invalid and will be ignored Required.
+      * **validationActions** ``List[str]`` - *(optional)* validationActions declares how Validations of the referenced
+        ValidatingAdmissionPolicy are enforced. If a validation evaluates to false it
+        is always enforced according to these actions.
+        Failures defined by the ValidatingAdmissionPolicy's FailurePolicy are enforced
+        according to these actions only if the FailurePolicy is set to Fail, otherwise
+        the failures are ignored. This includes compilation errors, runtime errors and
+        misconfigurations of the policy.
+        validationActions is declared as a set of action values. Order does not
+        matter. validationActions may not contain duplicates of the same action.
+        The supported actions values are:
+        "Deny" specifies that a validation failure results in a denied request.
+        "Warn" specifies that a validation failure is reported to the request client
+        in HTTP Warning headers, with a warning code of 299. Warnings can be sent both
+        for allowed or denied admission responses.
+        "Audit" specifies that a validation failure is included in the published audit
+        event for the request. The audit event will contain a
+        `validation.policy.admission.k8s.io/validation_failure` audit annotation with
+        a value containing the details of the validation failures, formatted as a JSON
+        list of objects, each with the following fields: - message: The validation
+        failure message string - policy: The resource name of the
+        ValidatingAdmissionPolicy - binding: The resource name of the
+        ValidatingAdmissionPolicyBinding - expressionIndex: The index of the failed
+        validations in the ValidatingAdmissionPolicy - validationActions: The
+        enforcement actions enacted for the validation failure Example audit
+        annotation: `"validation.policy.admission.k8s.io/validation_failure":
+        "[{"message": "Invalid value", {"policy": "policy.example.com", {"binding":
+        "policybinding.example.com", {"expressionIndex": "1", {"validationActions":
+        ["Audit"]}]"`
+        Clients should expect to handle additional values by ignoring any values not
+        recognized.
+        "Deny" and "Warn" may not be used together since this combination needlessly
+        duplicates the validation failure both in the API response body and the HTTP
+        warning headers.
+        Required.
     """
     matchResources: 'MatchResources' = None
     paramRef: 'ParamRef' = None
     policyName: 'str' = None
+    validationActions: 'List[str]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyList(DataclassDictMixIn):
     """ValidatingAdmissionPolicyList is a list of ValidatingAdmissionPolicy.
 
       **parameters**
@@ -290,56 +428,105 @@
 @dataclass
 class ValidatingAdmissionPolicySpec(DataclassDictMixIn):
     """ValidatingAdmissionPolicySpec is the specification of the desired behavior of
       the AdmissionPolicy.
 
       **parameters**
 
-      * **validations** ``List[Validation]`` - Validations contain CEL expressions which is used to apply the validation. A
-        minimum of one validation is required for a policy definition. Required.
-      * **failurePolicy** ``str`` - *(optional)* FailurePolicy defines how to handle failures for the admission policy.
-        Failures can occur from invalid or mis-configured policy definitions or
-        bindings. A policy is invalid if spec.paramKind refers to a non-existent Kind.
-        A binding is invalid if spec.paramRef.name refers to a non-existent resource.
+      * **auditAnnotations** ``List[AuditAnnotation]`` - *(optional)* auditAnnotations contains CEL expressions which are used to produce audit
+        annotations for the audit event of the API request. validations and
+        auditAnnotations may not both be empty; a least one of validations or
+        auditAnnotations is required.
+      * **failurePolicy** ``str`` - *(optional)* failurePolicy defines how to handle failures for the admission policy.
+        Failures can occur from CEL expression parse errors, type check errors,
+        runtime errors and invalid or mis-configured policy definitions or bindings.
+        A policy is invalid if spec.paramKind refers to a non-existent Kind. A binding
+        is invalid if spec.paramRef.name refers to a non-existent resource.
+        failurePolicy does not define how validations that evaluate to false are
+        handled.
+        When failurePolicy is set to Fail, ValidatingAdmissionPolicyBinding
+        validationActions define how failures are enforced.
         Allowed values are Ignore or Fail. Defaults to Fail.
+      * **matchConditions** ``List[MatchCondition]`` - *(optional)* MatchConditions is a list of conditions that must be met for a request to be
+        validated. Match conditions filter requests that have already been matched by
+        the rules, namespaceSelector, and objectSelector. An empty list of
+        matchConditions matches all requests. There are a maximum of 64 match
+        conditions allowed.
+        If a parameter object is provided, it can be accessed via the `params` handle
+        in the same manner as validation expressions.
+        The exact matching logic is (in order):
+          1. If ANY matchCondition evaluates to FALSE, the policy is skipped.
+          2. If ALL matchConditions evaluate to TRUE, the policy is evaluated.
+          3. If any matchCondition evaluates to an error (but none are FALSE):
+             - If failurePolicy=Fail, reject the request
+             - If failurePolicy=Ignore, the policy is skipped
       * **matchConstraints** ``MatchResources`` - *(optional)* MatchConstraints specifies what resources this policy is designed to validate.
         The AdmissionPolicy cares about a request if it matches _all_ Constraints.
         However, in order to prevent clusters from being put into an unstable state
         that cannot be recovered from via the API ValidatingAdmissionPolicy cannot
         match ValidatingAdmissionPolicy and ValidatingAdmissionPolicyBinding.
         Required.
       * **paramKind** ``ParamKind`` - *(optional)* ParamKind specifies the kind of resources used to parameterize this policy. If
         absent, there are no parameters for this policy and the param CEL variable
         will not be provided to validation expressions. If ParamKind refers to a
         non-existent kind, this policy definition is mis-configured and the
         FailurePolicy is applied. If paramKind is specified but paramRef is unset in
         ValidatingAdmissionPolicyBinding, the params variable will be null.
+      * **validations** ``List[Validation]`` - *(optional)* Validations contain CEL expressions which is used to apply the validation.
+        Validations and AuditAnnotations may not both be empty; a minimum of one
+        Validations or AuditAnnotations is required.
     """
-    validations: 'List[Validation]'
+    auditAnnotations: 'List[AuditAnnotation]' = None
     failurePolicy: 'str' = None
+    matchConditions: 'List[MatchCondition]' = None
     matchConstraints: 'MatchResources' = None
     paramKind: 'ParamKind' = None
+    validations: 'List[Validation]' = None
+
+
+@dataclass
+class ValidatingAdmissionPolicyStatus(DataclassDictMixIn):
+    """ValidatingAdmissionPolicyStatus represents the status of a
+      ValidatingAdmissionPolicy.
+
+      **parameters**
+
+      * **conditions** ``List[meta_v1.Condition]`` - *(optional)* The conditions represent the latest available observations of a policy's
+        current state.
+      * **observedGeneration** ``int`` - *(optional)* The generation observed by the controller.
+      * **typeChecking** ``TypeChecking`` - *(optional)* The results of type checking for each expression. Presence of this field
+        indicates the completion of the type checking.
+    """
+    conditions: 'List[meta_v1.Condition]' = None
+    observedGeneration: 'int' = None
+    typeChecking: 'TypeChecking' = None
 
 
 @dataclass
 class Validation(DataclassDictMixIn):
     """Validation specifies the CEL expression which is used to apply the validation.
 
       **parameters**
 
       * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. ref:
         https://github.com/google/cel-spec CEL expressions have access to the contents
-        of the Admission request/response, organized into CEL variables as well as
-        some other useful variables:
-        'object' - The object from the incoming request. The value is null for DELETE
-        requests. 'oldObject' - The existing object. The value is null for CREATE
-        requests. 'request' - Attributes of the admission
-        request([ref](/pkg/apis/admission/types.go#AdmissionRequest)). 'params' -
+        of the API request/response, organized into CEL variables as well as some
+        other useful variables:
+        - 'object' - The object from the incoming request. The value is null for
+        DELETE requests. - 'oldObject' - The existing object. The value is null for
+        CREATE requests. - 'request' - Attributes of the API
+        request([ref](/pkg/apis/admission/types.go#AdmissionRequest)). - 'params' -
         Parameter resource referred to by the policy binding being evaluated. Only
-        populated if the policy has a ParamKind.
+        populated if the policy has a ParamKind. - 'authorizer' - A CEL Authorizer.
+        May be used to perform authorization checks for the principal (user or service
+        account) of the request.
+          See https://pkg.go.dev/k8s.io/apiserver/pkg/cel/library#Authz
+        - 'authorizer.requestResource' - A CEL ResourceCheck constructed from the
+        'authorizer' and configured with the
+          request resource.
         The `apiVersion`, `kind`, `metadata.name` and `metadata.generateName` are
         always accessible from the root of the object. No other metadata properties
         are accessible.
         Only property names of the form `[a-zA-Z_.-/][a-zA-Z0-9_.-/]*` are accessible.
         Accessible property names are escaped according to the following rules when
         accessed in the expression: - '__' escapes to '__underscores__' - '.' escapes
         to '__dot__' - '-' escapes to '__dash__' - '/' escapes to '__slash__' -
@@ -370,19 +557,34 @@
         Required.
       * **message** ``str`` - *(optional)* Message represents the message displayed when validation fails. The message is
         required if the Expression contains line breaks. The message must not contain
         line breaks. If unset, the message is "failed rule: {Rule}". e.g. "must be a
         URL with the host matching spec.host" If the Expression contains line breaks.
         Message is required. The message must not contain line breaks. If unset, the
         message is "failed Expression: {Expression}".
+      * **messageExpression** ``str`` - *(optional)* messageExpression declares a CEL expression that evaluates to the validation
+        failure message that is returned when this rule fails. Since messageExpression
+        is used as a failure message, it must evaluate to a string. If both message
+        and messageExpression are present on a validation, then messageExpression will
+        be used if validation fails. If messageExpression results in a runtime error,
+        the runtime error is logged, and the validation failure message is produced as
+        if the messageExpression field were unset. If messageExpression evaluates to
+        an empty string, a string with only spaces, or a string that contains line
+        breaks, then the validation failure message will also be produced as if the
+        messageExpression field were unset, and the fact that messageExpression
+        produced an empty string/string with only spaces/string with line breaks will
+        be logged. messageExpression has access to all the same variables as the
+        `expression` except for 'authorizer' and 'authorizer.requestResource'.
+        Example: "object.x must be less than max ("+string(params.max)+")"
       * **reason** ``str`` - *(optional)* Reason represents a machine-readable description of why this validation
         failed. If this is the first validation in the list to fail, this reason, as
         well as the corresponding HTTP response code, are used in the HTTP response to
         the client. The currently supported reasons are: "Unauthorized", "Forbidden",
         "Invalid", "RequestEntityTooLarge". If not set, StatusReasonInvalid is used in
         the response to the client.
     """
     expression: 'str'
     message: 'str' = None
+    messageExpression: 'str' = None
     reason: 'str' = None
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/apiextensions_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/apiextensions_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from typing import Any
 from . import meta_v1
 from typing import Dict
+from typing import Any
 
 
 @dataclass
 class CustomResourceColumnDefinition(DataclassDictMixIn):
     """CustomResourceColumnDefinition specifies a column for server side printing.
 
       **parameters**
@@ -43,22 +43,22 @@
 @dataclass
 class CustomResourceConversion(DataclassDictMixIn):
     """CustomResourceConversion describes how to convert different versions of a CR.
 
       **parameters**
 
       * **strategy** ``str`` - strategy specifies how custom resources are converted between versions.
-        Allowed values are: - `None`: The converter only change the apiVersion and
-        would not touch any other field in the custom resource. - `Webhook`: API
+        Allowed values are: - `"None"`: The converter only change the apiVersion and
+        would not touch any other field in the custom resource. - `"Webhook"`: API
         Server will call to an external webhook to do the conversion. Additional
         information
           is needed for this option. This requires spec.preserveUnknownFields to be
         false, and spec.conversion.webhook to be set.
       * **webhook** ``WebhookConversion`` - *(optional)* webhook describes how to call the conversion webhook. Required when `strategy`
-        is set to `Webhook`.
+        is set to `"Webhook"`.
     """
     strategy: 'str'
     webhook: 'WebhookConversion' = None
 
 
 @dataclass
 class CustomResourceDefinition(DataclassDictMixIn):
@@ -631,17 +631,32 @@
             are overwritten by values in `Y` when the key sets of `X` and `Y`
         intersect. Elements in `Y` with
             non-intersecting keys are appended, retaining their partial order.
       * **message** ``str`` - *(optional)* Message represents the message displayed when validation fails. The message is
         required if the Rule contains line breaks. The message must not contain line
         breaks. If unset, the message is "failed rule: {Rule}". e.g. "must be a URL
         with the host matching spec.host"
+      * **messageExpression** ``str`` - *(optional)* MessageExpression declares a CEL expression that evaluates to the validation
+        failure message that is returned when this rule fails. Since messageExpression
+        is used as a failure message, it must evaluate to a string. If both message
+        and messageExpression are present on a rule, then messageExpression will be
+        used if validation fails. If messageExpression results in a runtime error, the
+        runtime error is logged, and the validation failure message is produced as if
+        the messageExpression field were unset. If messageExpression evaluates to an
+        empty string, a string with only spaces, or a string that contains line
+        breaks, then the validation failure message will also be produced as if the
+        messageExpression field were unset, and the fact that messageExpression
+        produced an empty string/string with only spaces/string with line breaks will
+        be logged. messageExpression has access to all the same variables as the rule;
+        the only difference is the return type. Example: "x must be less than max
+        ("+string(self.max)+")"
     """
     rule: 'str'
     message: 'str' = None
+    messageExpression: 'str' = None
 
 
 @dataclass
 class WebhookClientConfig(DataclassDictMixIn):
     """WebhookClientConfig contains the information to make a TLS connection with the
       webhook.
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/apiregistration_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/apiregistration_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/models/apiserverinternal_v1alpha1.py` & `lightkube-models-1.27.1.4/lightkube/models/apiserverinternal_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/models/apps_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/apps_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from . import util_intstr
-from . import runtime
 from . import meta_v1
 from . import core_v1
+from . import util_intstr
+from . import runtime
 
 
 @dataclass
 class ControllerRevision(DataclassDictMixIn):
     """ControllerRevision implements an immutable snapshot of state data. Clients are
       responsible for serializing and deserializing the objects that contain their
       internal state. Once a ControllerRevision has been successfully created, it
@@ -149,15 +149,16 @@
       **parameters**
 
       * **selector** ``meta_v1.LabelSelector`` - A label query over pods that are managed by the daemon set. Must match in
         order to be controlled. It must match the pod template's labels. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors
       * **template** ``core_v1.PodTemplateSpec`` - An object that describes the pod that will be created. The DaemonSet will
         create exactly one copy of this pod on every node that matches the template's
-        node selector (or on every node if no node selector is specified). More info:
+        node selector (or on every node if no node selector is specified). The only
+        allowed template.spec.restartPolicy value is "Always". More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller#pod-template
       * **minReadySeconds** ``int`` - *(optional)* The minimum number of seconds for which a newly created DaemonSet pod should
         be ready without any of its container crashing, for it to be considered
         available. Defaults to 0 (pod will be considered available as soon as it is
         ready).
       * **revisionHistoryLimit** ``int`` - *(optional)* The number of old history to retain to allow rollback. This is a pointer to
         distinguish between explicit zero and not specified. Defaults to 10.
@@ -301,15 +302,16 @@
     """DeploymentSpec is the specification of the desired behavior of the Deployment.
 
       **parameters**
 
       * **selector** ``meta_v1.LabelSelector`` - Label selector for pods. Existing ReplicaSets whose pods are selected by this
         will be the ones affected by this deployment. It must match the pod template's
         labels.
-      * **template** ``core_v1.PodTemplateSpec`` - Template describes the pods that will be created.
+      * **template** ``core_v1.PodTemplateSpec`` - Template describes the pods that will be created. The only allowed
+        template.spec.restartPolicy value is "Always".
       * **minReadySeconds** ``int`` - *(optional)* Minimum number of seconds for which a newly created pod should be ready
         without any of its container crashing, for it to be considered available.
         Defaults to 0 (pod will be considered available as soon as it is ready)
       * **paused** ``bool`` - *(optional)* Indicates that the deployment is paused.
       * **progressDeadlineSeconds** ``int`` - *(optional)* The maximum time in seconds for a deployment to make progress before it is
         considered to be failed. The deployment controller will continue to process
         failed deployments and a condition with a ProgressDeadlineExceeded reason will
@@ -731,23 +733,24 @@
         pod-specific-string.serviceName.default.svc.cluster.local where
         "pod-specific-string" is managed by the StatefulSet controller.
       * **template** ``core_v1.PodTemplateSpec`` - template is the object that describes the pod that will be created if
         insufficient replicas are detected. Each pod stamped out by the StatefulSet
         will fulfill this Template, but have a unique identity from the rest of the
         StatefulSet. Each pod will be named with the format
         <statefulsetname>-<podindex>. For example, a pod in a StatefulSet named "web"
-        with index number "3" would be named "web-3".
+        with index number "3" would be named "web-3". The only allowed
+        template.spec.restartPolicy value is "Always".
       * **minReadySeconds** ``int`` - *(optional)* Minimum number of seconds for which a newly created pod should be ready
         without any of its container crashing for it to be considered available.
         Defaults to 0 (pod will be considered available as soon as it is ready)
       * **ordinals** ``StatefulSetOrdinals`` - *(optional)* ordinals controls the numbering of replica indices in a StatefulSet. The
         default ordinals behavior assigns a "0" index to the first replica and
         increments the index by one for each additional replica requested. Using the
         ordinals field requires the StatefulSetStartOrdinal feature gate to be
-        enabled, which is alpha.
+        enabled, which is beta.
       * **persistentVolumeClaimRetentionPolicy** ``StatefulSetPersistentVolumeClaimRetentionPolicy`` - *(optional)* persistentVolumeClaimRetentionPolicy describes the lifecycle of persistent
         volume claims created from volumeClaimTemplates. By default, all persistent
         volume claims are created as needed and retained until manually deleted. This
         policy allows the lifecycle to be altered, for example by deleting persistent
         volume claims when their stateful set is deleted, or when their pod is scaled
         down. This requires the StatefulSetAutoDeletePVC feature gate to be enabled,
         which is alpha.  +optional
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/authentication_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/authentication_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/models/authentication_v1alpha1.py` & `lightkube-models-1.27.1.4/lightkube/models/authentication_v1alpha1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from . import authentication_v1
 from . import meta_v1
+from . import authentication_v1
 
 
 @dataclass
 class SelfSubjectReview(DataclassDictMixIn):
     """SelfSubjectReview contains the user information that the kube-apiserver has
       about the user making this request. When using impersonation, users will
-      receive the user info of the user being impersonated.
+      receive the user info of the user being impersonated.  If impersonation or
+      request header authentication is used, any extra keys will have their case
+      ignored and returned as lowercase.
 
       **parameters**
 
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/authorization_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/authorization_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/models/autoscaling_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/autoscaling_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 @dataclass
 class CrossVersionObjectReference(DataclassDictMixIn):
     """CrossVersionObjectReference contains enough information to let you identify
       the referred resource.
 
       **parameters**
 
-      * **kind** ``str`` - Kind of the referent; More info:
+      * **kind** ``str`` - kind is the kind of the referent; More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **name** ``str`` - Name of the referent; More info:
-        http://kubernetes.io/docs/user-guide/identifiers#names
-      * **apiVersion** ``str`` - *(optional)* API version of the referent
+      * **name** ``str`` - name is the name of the referent; More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names
+      * **apiVersion** ``str`` - *(optional)* apiVersion is the API version of the referent
     """
     kind: 'str'
     name: 'str'
     apiVersion: 'str' = None
 
 
 @dataclass
@@ -37,32 +37,32 @@
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object metadata. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **spec** ``HorizontalPodAutoscalerSpec`` - *(optional)* behaviour of autoscaler. More info:
+      * **spec** ``HorizontalPodAutoscalerSpec`` - *(optional)* spec defines the behaviour of autoscaler. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status.
-      * **status** ``HorizontalPodAutoscalerStatus`` - *(optional)* current information about the autoscaler.
+      * **status** ``HorizontalPodAutoscalerStatus`` - *(optional)* status is the current information about the autoscaler.
     """
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
     spec: 'HorizontalPodAutoscalerSpec' = None
     status: 'HorizontalPodAutoscalerStatus' = None
 
 
 @dataclass
 class HorizontalPodAutoscalerList(DataclassDictMixIn):
     """list of horizontal pod autoscaler objects.
 
       **parameters**
 
-      * **items** ``List[HorizontalPodAutoscaler]`` - list of horizontal pod autoscaler objects.
+      * **items** ``List[HorizontalPodAutoscaler]`` - items is the list of horizontal pod autoscaler objects.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
@@ -77,48 +77,51 @@
 
 @dataclass
 class HorizontalPodAutoscalerSpec(DataclassDictMixIn):
     """specification of a horizontal pod autoscaler.
 
       **parameters**
 
-      * **maxReplicas** ``int`` - upper limit for the number of pods that can be set by the autoscaler; cannot
-        be smaller than MinReplicas.
+      * **maxReplicas** ``int`` - maxReplicas is the upper limit for the number of pods that can be set by the
+        autoscaler; cannot be smaller than MinReplicas.
       * **scaleTargetRef** ``CrossVersionObjectReference`` - reference to scaled resource; horizontal pod autoscaler will learn the current
         resource consumption and will set the desired number of pods by using its
         Scale subresource.
       * **minReplicas** ``int`` - *(optional)* minReplicas is the lower limit for the number of replicas to which the
         autoscaler can scale down.  It defaults to 1 pod.  minReplicas is allowed to
         be 0 if the alpha feature gate HPAScaleToZero is enabled and at least one
         Object or External metric is configured.  Scaling is active as long as at
         least one metric value is available.
-      * **targetCPUUtilizationPercentage** ``int`` - *(optional)* target average CPU utilization (represented as a percentage of requested CPU)
-        over all the pods; if not specified the default autoscaling policy will be
-        used.
+      * **targetCPUUtilizationPercentage** ``int`` - *(optional)* targetCPUUtilizationPercentage is the target average CPU utilization
+        (represented as a percentage of requested CPU) over all the pods; if not
+        specified the default autoscaling policy will be used.
     """
     maxReplicas: 'int'
     scaleTargetRef: 'CrossVersionObjectReference'
     minReplicas: 'int' = None
     targetCPUUtilizationPercentage: 'int' = None
 
 
 @dataclass
 class HorizontalPodAutoscalerStatus(DataclassDictMixIn):
     """current status of a horizontal pod autoscaler
 
       **parameters**
 
-      * **currentReplicas** ``int`` - current number of replicas of pods managed by this autoscaler.
-      * **desiredReplicas** ``int`` - desired number of replicas of pods managed by this autoscaler.
-      * **currentCPUUtilizationPercentage** ``int`` - *(optional)* current average CPU utilization over all pods, represented as a percentage of
-        requested CPU, e.g. 70 means that an average pod is using now 70% of its
-        requested CPU.
-      * **lastScaleTime** ``meta_v1.Time`` - *(optional)* last time the HorizontalPodAutoscaler scaled the number of pods; used by the
-        autoscaler to control how often the number of pods is changed.
-      * **observedGeneration** ``int`` - *(optional)* most recent generation observed by this autoscaler.
+      * **currentReplicas** ``int`` - currentReplicas is the current number of replicas of pods managed by this
+        autoscaler.
+      * **desiredReplicas** ``int`` - desiredReplicas is the  desired number of replicas of pods managed by this
+        autoscaler.
+      * **currentCPUUtilizationPercentage** ``int`` - *(optional)* currentCPUUtilizationPercentage is the current average CPU utilization over
+        all pods, represented as a percentage of requested CPU, e.g. 70 means that an
+        average pod is using now 70% of its requested CPU.
+      * **lastScaleTime** ``meta_v1.Time`` - *(optional)* lastScaleTime is the last time the HorizontalPodAutoscaler scaled the number
+        of pods; used by the autoscaler to control how often the number of pods is
+        changed.
+      * **observedGeneration** ``int`` - *(optional)* observedGeneration is the most recent generation observed by this autoscaler.
     """
     currentReplicas: 'int'
     desiredReplicas: 'int'
     currentCPUUtilizationPercentage: 'int' = None
     lastScaleTime: 'meta_v1.Time' = None
     observedGeneration: 'int' = None
 
@@ -135,17 +138,17 @@
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object metadata; More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.
-      * **spec** ``ScaleSpec`` - *(optional)* defines the behavior of the scale. More info:
+      * **spec** ``ScaleSpec`` - *(optional)* spec defines the behavior of the scale. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status.
-      * **status** ``ScaleStatus`` - *(optional)* current status of the scale. More info:
+      * **status** ``ScaleStatus`` - *(optional)* status is the current status of the scale. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status.
         Read-only.
     """
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
     spec: 'ScaleSpec' = None
@@ -154,29 +157,29 @@
 
 @dataclass
 class ScaleSpec(DataclassDictMixIn):
     """ScaleSpec describes the attributes of a scale subresource.
 
       **parameters**
 
-      * **replicas** ``int`` - *(optional)* desired number of instances for the scaled object.
+      * **replicas** ``int`` - *(optional)* replicas is the desired number of instances for the scaled object.
     """
     replicas: 'int' = None
 
 
 @dataclass
 class ScaleStatus(DataclassDictMixIn):
     """ScaleStatus represents the current status of a scale subresource.
 
       **parameters**
 
-      * **replicas** ``int`` - actual number of observed instances of the scaled object.
-      * **selector** ``str`` - *(optional)* label query over pods that should match the replicas count. This is same as
-        the label selector but in the string format to avoid introspection by clients.
-        The string will be in the same format as the query-param syntax. More info
-        about label selectors:
-        http://kubernetes.io/docs/user-guide/labels#label-selectors
+      * **replicas** ``int`` - replicas is the actual number of observed instances of the scaled object.
+      * **selector** ``str`` - *(optional)* selector is the label query over pods that should match the replicas count.
+        This is same as the label selector but in the string format to avoid
+        introspection by clients. The string will be in the same format as the
+        query-param syntax. More info about label selectors:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/
     """
     replicas: 'int'
     selector: 'str' = None
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/autoscaling_v2.py` & `lightkube-models-1.27.1.4/lightkube/models/autoscaling_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,35 +35,35 @@
       known to Kubernetes, as specified in requests and limits, describing a single
       container in each pod in the current scale target (e.g. CPU or memory).  Such
       metrics are built in to Kubernetes, and have special scaling options on top of
       those available to normal per-pod metrics using the "pods" source.
 
       **parameters**
 
-      * **container** ``str`` - Container is the name of the container in the pods of the scaling target
+      * **container** ``str`` - container is the name of the container in the pods of the scaling target
       * **current** ``MetricValueStatus`` - current contains the current value for the given metric
-      * **name** ``str`` - Name is the name of the resource in question.
+      * **name** ``str`` - name is the name of the resource in question.
     """
     container: 'str'
     current: 'MetricValueStatus'
     name: 'str'
 
 
 @dataclass
 class CrossVersionObjectReference(DataclassDictMixIn):
     """CrossVersionObjectReference contains enough information to let you identify
       the referred resource.
 
       **parameters**
 
-      * **kind** ``str`` - Kind of the referent; More info:
+      * **kind** ``str`` - kind is the kind of the referent; More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **name** ``str`` - Name of the referent; More info:
-        http://kubernetes.io/docs/user-guide/identifiers#names
-      * **apiVersion** ``str`` - *(optional)* API version of the referent
+      * **name** ``str`` - name is the name of the referent; More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names
+      * **apiVersion** ``str`` - *(optional)* apiVersion is the API version of the referent
     """
     kind: 'str'
     name: 'str'
     apiVersion: 'str' = None
 
 
 @dataclass
@@ -98,19 +98,19 @@
 @dataclass
 class HPAScalingPolicy(DataclassDictMixIn):
     """HPAScalingPolicy is a single policy which must hold true for a specified past
       interval.
 
       **parameters**
 
-      * **periodSeconds** ``int`` - PeriodSeconds specifies the window of time for which the policy should hold
+      * **periodSeconds** ``int`` - periodSeconds specifies the window of time for which the policy should hold
         true. PeriodSeconds must be greater than zero and less than or equal to 1800
         (30 min).
-      * **type** ``str`` - Type is used to specify the scaling policy.
-      * **value** ``int`` - Value contains the amount of change which is permitted by the policy. It must
+      * **type** ``str`` - type is used to specify the scaling policy.
+      * **value** ``int`` - value contains the amount of change which is permitted by the policy. It must
         be greater than zero
     """
     periodSeconds: 'int'
     type: 'str'
     value: 'int'
 
 
@@ -126,15 +126,15 @@
       **parameters**
 
       * **policies** ``List[HPAScalingPolicy]`` - *(optional)* policies is a list of potential scaling polices which can be used during
         scaling. At least one policy must be specified, otherwise the HPAScalingRules
         will be discarded as invalid
       * **selectPolicy** ``str`` - *(optional)* selectPolicy is used to specify which policy should be used. If not set, the
         default value Max is used.
-      * **stabilizationWindowSeconds** ``int`` - *(optional)* StabilizationWindowSeconds is the number of seconds for which past
+      * **stabilizationWindowSeconds** ``int`` - *(optional)* stabilizationWindowSeconds is the number of seconds for which past
         recommendations should be considered while scaling up or scaling down.
         StabilizationWindowSeconds must be greater than or equal to zero and less than
         or equal to 3600 (one hour). If not set, use the default values: - For scale
         up: 0 (i.e. no stabilization is done). - For scale down: 300 (i.e. the
         stabilization window is 300 seconds long).
     """
     policies: 'List[HPAScalingPolicy]' = None
@@ -522,13 +522,13 @@
       current scale target (e.g. CPU or memory).  Such metrics are built in to
       Kubernetes, and have special scaling options on top of those available to
       normal per-pod metrics using the "pods" source.
 
       **parameters**
 
       * **current** ``MetricValueStatus`` - current contains the current value for the given metric
-      * **name** ``str`` - Name is the name of the resource in question.
+      * **name** ``str`` - name is the name of the resource in question.
     """
     current: 'MetricValueStatus'
     name: 'str'
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/batch_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/batch_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from . import core_v1
 from . import meta_v1
+from . import core_v1
 
 
 @dataclass
 class CronJob(DataclassDictMixIn):
     """CronJob represents the configuration of a single cron job.
 
       **parameters**
@@ -66,16 +66,16 @@
     """CronJobSpec describes how the job execution will look like and when it will
       actually run.
 
       **parameters**
 
       * **jobTemplate** ``JobTemplateSpec`` - Specifies the job that will be created when executing a CronJob.
       * **schedule** ``str`` - The schedule in Cron format, see https://en.wikipedia.org/wiki/Cron.
-      * **concurrencyPolicy** ``str`` - *(optional)* Specifies how to treat concurrent executions of a Job. Valid values are: -
-        "Allow" (default): allows CronJobs to run concurrently; - "Forbid": forbids
+      * **concurrencyPolicy** ``str`` - *(optional)* Specifies how to treat concurrent executions of a Job. Valid values are:
+        - "Allow" (default): allows CronJobs to run concurrently; - "Forbid": forbids
         concurrent runs, skipping next run if previous run hasn't finished yet; -
         "Replace": cancels currently running job and replaces it with a new one
       * **failedJobsHistoryLimit** ``int`` - *(optional)* The number of failed finished jobs to retain. Value must be non-negative
         integer. Defaults to 1.
       * **startingDeadlineSeconds** ``int`` - *(optional)* Optional deadline in seconds for starting the job if it misses scheduled time
         for any reason.  Missed jobs executions will be counted as failed ones.
       * **successfulJobsHistoryLimit** ``int`` - *(optional)* The number of successful finished jobs to retain. Value must be non-negative
@@ -90,15 +90,14 @@
         validation and the controller manager during execution. If no system-wide time
         zone database can be found a bundled version of the database is used instead.
         If the time zone name becomes invalid during the lifetime of a CronJob or due
         to a change in host configuration, the controller will stop creating new new
         Jobs and will create a system event with the reason UnknownTimeZone. More
         information can be found in
         https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/#time-zones
-        This is beta field and must be enabled via the `CronJobTimeZone` feature gate.
     """
     jobTemplate: 'JobTemplateSpec'
     schedule: 'str'
     concurrencyPolicy: 'str' = None
     failedJobsHistoryLimit: 'int' = None
     startingDeadlineSeconds: 'int' = None
     successfulJobsHistoryLimit: 'int' = None
@@ -196,23 +195,24 @@
 
 @dataclass
 class JobSpec(DataclassDictMixIn):
     """JobSpec describes how the job execution will look like.
 
       **parameters**
 
-      * **template** ``core_v1.PodTemplateSpec`` - Describes the pod that will be created when executing a job. More info:
+      * **template** ``core_v1.PodTemplateSpec`` - Describes the pod that will be created when executing a job. The only allowed
+        template.spec.restartPolicy values are "Never" or "OnFailure". More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/jobs-run-to-completion/
       * **activeDeadlineSeconds** ``int`` - *(optional)* Specifies the duration in seconds relative to the startTime that the job may
         be continuously active before the system tries to terminate it; value must be
         positive integer. If a Job is suspended (at creation or through an update),
         this timer will effectively be stopped and reset when the Job is resumed
         again.
       * **backoffLimit** ``int`` - *(optional)* Specifies the number of retries before marking this job failed. Defaults to 6
-      * **completionMode** ``str`` - *(optional)* CompletionMode specifies how Pod completions are tracked. It can be
+      * **completionMode** ``str`` - *(optional)* completionMode specifies how Pod completions are tracked. It can be
         `NonIndexed` (default) or `Indexed`.
         `NonIndexed` means that the Job is considered complete when there have been
         .spec.completions successfully completed Pods. Each Pod completion is
         homologous to each other.
         `Indexed` means that the Pods of a Job get an associated completion index from
         0 to (.spec.completions - 1), available in the annotation
         batch.kubernetes.io/job-completion-index. The Job is considered complete when
@@ -221,15 +221,15 @@
         less than or equal to 10^5. In addition, The Pod name takes the form
         `$(job-name)-$(index)-$(random-string)`, the Pod hostname takes the form
         `$(job-name)-$(index)`.
         More completion modes can be added in the future. If the Job controller
         observes a mode that it doesn't recognize, which is possible during upgrades
         due to version skew, the controller skips updates for the Job.
       * **completions** ``int`` - *(optional)* Specifies the desired number of successfully finished pods the job should be
-        run with.  Setting to nil means that the success of any pod signals the
+        run with.  Setting to null means that the success of any pod signals the
         success of all pods, and allows parallelism to have any positive value.
         Setting to 1 means that parallelism is limited to 1 and the success of that
         pod signals the success of the job. More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/jobs-run-to-completion/
       * **manualSelector** ``bool`` - *(optional)* manualSelector controls generation of pod labels and pod selectors. Leave
         `manualSelector` unset unless you are certain what you are doing. When false
         or unset, the system pick labels unique to this job and appends those labels
@@ -251,15 +251,15 @@
         and it is checked against the backoffLimit. This field cannot be used in
         combination with restartPolicy=OnFailure.
         This field is alpha-level. To use this field, you must enable the
         `JobPodFailurePolicy` feature gate (disabled by default).
       * **selector** ``meta_v1.LabelSelector`` - *(optional)* A label query over pods that should match the pod count. Normally, the system
         sets this field for you. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors
-      * **suspend** ``bool`` - *(optional)* Suspend specifies whether the Job controller should create Pods or not. If a
+      * **suspend** ``bool`` - *(optional)* suspend specifies whether the Job controller should create Pods or not. If a
         Job is created with suspend set to true, no Pods are created by the Job
         controller. If a Job is suspended after creation (i.e. the flag goes from
         false to true), the Job controller will delete all active Pods associated with
         this Job. Users must design their workload to gracefully handle this.
         Suspending a Job will reset the StartTime field of the Job, effectively
         resetting the ActiveDeadlineSeconds timer too. Defaults to false.
       * **ttlSecondsAfterFinished** ``int`` - *(optional)* ttlSecondsAfterFinished limits the lifetime of a Job that has finished
@@ -286,15 +286,15 @@
 @dataclass
 class JobStatus(DataclassDictMixIn):
     """JobStatus represents the current state of a Job.
 
       **parameters**
 
       * **active** ``int`` - *(optional)* The number of pending and running pods.
-      * **completedIndexes** ``str`` - *(optional)* CompletedIndexes holds the completed indexes when .spec.completionMode =
+      * **completedIndexes** ``str`` - *(optional)* completedIndexes holds the completed indexes when .spec.completionMode =
         "Indexed" in a text format. The indexes are represented as decimal integers
         separated by commas. The numbers are listed in increasing order. Three or more
         consecutive numbers are compressed and represented by the first and last
         element of the series, separated by a hyphen. For example, if the completed
         indexes are 1, 3, 4, 5 and 7, they are represented as "1,3-5,7".
       * **completionTime** ``meta_v1.Time`` - *(optional)* Represents time when the job was completed. It is not guaranteed to be set in
         happens-before order across separate operations. It is represented in RFC3339
@@ -312,21 +312,21 @@
         This field is beta-level. The job controller populates the field when the
         feature gate JobReadyPods is enabled (enabled by default).
       * **startTime** ``meta_v1.Time`` - *(optional)* Represents time when the job controller started processing a job. When a Job
         is created in the suspended state, this field is not set until the first time
         it is resumed. This field is reset every time a Job is resumed from
         suspension. It is represented in RFC3339 form and is in UTC.
       * **succeeded** ``int`` - *(optional)* The number of pods which reached phase Succeeded.
-      * **uncountedTerminatedPods** ``UncountedTerminatedPods`` - *(optional)* UncountedTerminatedPods holds the UIDs of Pods that have terminated but the
+      * **uncountedTerminatedPods** ``UncountedTerminatedPods`` - *(optional)* uncountedTerminatedPods holds the UIDs of Pods that have terminated but the
         job controller hasn't yet accounted for in the status counters.
         The job controller creates pods with a finalizer. When a pod terminates
         (succeeded or failed), the controller does three steps to account for it in
-        the job status: (1) Add the pod UID to the arrays in this field. (2) Remove
-        the pod finalizer. (3) Remove the pod UID from the arrays while increasing the
-        corresponding
+        the job status:
+        1. Add the pod UID to the arrays in this field. 2. Remove the pod finalizer.
+        3. Remove the pod UID from the arrays while increasing the corresponding
             counter.
         Old jobs might not be tracked using this field, in which case the field
         remains null.
     """
     active: 'int' = None
     completedIndexes: 'str' = None
     completionTime: 'meta_v1.Time' = None
@@ -378,16 +378,16 @@
       fields in the Pod status, respectively. Containers completed with success
       (exit code 0) are excluded from the requirement check.
 
       **parameters**
 
       * **operator** ``str`` - Represents the relationship between the container exit code(s) and the
         specified values. Containers completed with success (exit code 0) are excluded
-        from the requirement check. Possible values are: - In: the requirement is
-        satisfied if at least one container exit code
+        from the requirement check. Possible values are:
+        - In: the requirement is satisfied if at least one container exit code
           (might be multiple if there are multiple containers not restricted
           by the 'containerName' field) is in the set of specified values.
         - NotIn: the requirement is satisfied if at least one container exit code
           (might be multiple if there are multiple containers not restricted
           by the 'containerName' field) is not in the set of specified values.
         Additional values are considered to be added in the future. Clients should
         react to an unknown operator by assuming the requirement is not satisfied.
@@ -421,22 +421,22 @@
     status: 'str'
     type: 'str'
 
 
 @dataclass
 class PodFailurePolicyRule(DataclassDictMixIn):
     """PodFailurePolicyRule describes how a pod failure is handled when the
-      requirements are met. One of OnExitCodes and onPodConditions, but not both,
+      requirements are met. One of onExitCodes and onPodConditions, but not both,
       can be used in each rule.
 
       **parameters**
 
       * **action** ``str`` - Specifies the action taken on a pod failure when the requirements are
-        satisfied. Possible values are: - FailJob: indicates that the pod's job is
-        marked as Failed and all
+        satisfied. Possible values are:
+        - FailJob: indicates that the pod's job is marked as Failed and all
           running pods are terminated.
         - Ignore: indicates that the counter towards the .backoffLimit is not
           incremented and a replacement pod is created.
         - Count: indicates that the pod is handled in the default way - the
           counter towards the .backoffLimit is incremented.
         Additional values are considered to be added in the future. Clients should
         react to an unknown action by skipping the rule.
@@ -454,14 +454,14 @@
 @dataclass
 class UncountedTerminatedPods(DataclassDictMixIn):
     """UncountedTerminatedPods holds UIDs of Pods that have terminated but haven't
       been accounted in Job status counters.
 
       **parameters**
 
-      * **failed** ``List[str]`` - *(optional)* Failed holds UIDs of failed Pods.
-      * **succeeded** ``List[str]`` - *(optional)* Succeeded holds UIDs of succeeded Pods.
+      * **failed** ``List[str]`` - *(optional)* failed holds UIDs of failed Pods.
+      * **succeeded** ``List[str]`` - *(optional)* succeeded holds UIDs of succeeded Pods.
     """
     failed: 'List[str]' = None
     succeeded: 'List[str]' = None
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/certificates_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/certificates_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/models/coordination_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/coordination_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,30 +19,30 @@
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **spec** ``LeaseSpec`` - *(optional)* Specification of the Lease. More info:
+      * **spec** ``LeaseSpec`` - *(optional)* spec contains the specification of the Lease. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status
     """
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
     spec: 'LeaseSpec' = None
 
 
 @dataclass
 class LeaseList(DataclassDictMixIn):
     """LeaseList is a list of Lease objects.
 
       **parameters**
 
-      * **items** ``List[Lease]`` - Items is a list of schema objects.
+      * **items** ``List[Lease]`` - items is a list of schema objects.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
@@ -61,15 +61,15 @@
     """LeaseSpec is a specification of a Lease.
 
       **parameters**
 
       * **acquireTime** ``meta_v1.MicroTime`` - *(optional)* acquireTime is a time when the current lease was acquired.
       * **holderIdentity** ``str`` - *(optional)* holderIdentity contains the identity of the holder of a current lease.
       * **leaseDurationSeconds** ``int`` - *(optional)* leaseDurationSeconds is a duration that candidates for a lease need to wait to
-        force acquire it. This is measure against time of last observed RenewTime.
+        force acquire it. This is measure against time of last observed renewTime.
       * **leaseTransitions** ``int`` - *(optional)* leaseTransitions is the number of transitions of a lease between holders.
       * **renewTime** ``meta_v1.MicroTime`` - *(optional)* renewTime is a time when the current holder of a lease has last updated the
         lease.
     """
     acquireTime: 'meta_v1.MicroTime' = None
     holderIdentity: 'str' = None
     leaseDurationSeconds: 'int' = None
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/core_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/core_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
+from . import resource
 from . import util_intstr
 from . import meta_v1
-from . import resource
 
 
 @dataclass
 class AWSElasticBlockStoreVolumeSource(DataclassDictMixIn):
     """Represents a Persistent Disk resource in AWS.
       
       An AWS EBS disk must exist before mounting to a container. The disk must also
@@ -171,30 +171,29 @@
       **parameters**
 
       * **driver** ``str`` - driver is the name of the driver to use for this volume. Required.
       * **volumeHandle** ``str`` - volumeHandle is the unique volume name returned by the CSI volume plugin’s
         CreateVolume to refer to the volume on all subsequent calls. Required.
       * **controllerExpandSecretRef** ``SecretReference`` - *(optional)* controllerExpandSecretRef is a reference to the secret object containing
         sensitive information to pass to the CSI driver to complete the CSI
-        ControllerExpandVolume call. This is an beta field and requires enabling
-        ExpandCSIVolumes feature gate. This field is optional, and may be empty if no
+        ControllerExpandVolume call. This field is optional, and may be empty if no
         secret is required. If the secret object contains more than one secret, all
         secrets are passed.
       * **controllerPublishSecretRef** ``SecretReference`` - *(optional)* controllerPublishSecretRef is a reference to the secret object containing
         sensitive information to pass to the CSI driver to complete the CSI
         ControllerPublishVolume and ControllerUnpublishVolume calls. This field is
         optional, and may be empty if no secret is required. If the secret object
         contains more than one secret, all secrets are passed.
       * **fsType** ``str`` - *(optional)* fsType to mount. Must be a filesystem type supported by the host operating
         system. Ex. "ext4", "xfs", "ntfs".
       * **nodeExpandSecretRef** ``SecretReference`` - *(optional)* nodeExpandSecretRef is a reference to the secret object containing sensitive
         information to pass to the CSI driver to complete the CSI NodeExpandVolume
-        call. This is an alpha field and requires enabling CSINodeExpandSecret feature
-        gate. This field is optional, may be omitted if no secret is required. If the
-        secret object contains more than one secret, all secrets are passed.
+        call. This is a beta field which is enabled default by CSINodeExpandSecret
+        feature gate. This field is optional, may be omitted if no secret is required.
+        If the secret object contains more than one secret, all secrets are passed.
       * **nodePublishSecretRef** ``SecretReference`` - *(optional)* nodePublishSecretRef is a reference to the secret object containing sensitive
         information to pass to the CSI driver to complete the CSI NodePublishVolume
         and NodeUnpublishVolume calls. This field is optional, and may be empty if no
         secret is required. If the secret object contains more than one secret, all
         secrets are passed.
       * **nodeStageSecretRef** ``SecretReference`` - *(optional)* nodeStageSecretRef is a reference to the secret object containing sensitive
         information to pass to the CSI driver to complete the CSI NodeStageVolume and
@@ -721,14 +720,15 @@
         default "0.0.0.0" address inside a container will be accessible from the
         network. Modifying this array with strategic merge patch may corrupt the data.
         For more information See
         https://github.com/kubernetes/kubernetes/issues/108255. Cannot be updated.
       * **readinessProbe** ``Probe`` - *(optional)* Periodic probe of container service readiness. Container will be removed from
         service endpoints if the probe fails. Cannot be updated. More info:
         https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes
+      * **resizePolicy** ``List[ContainerResizePolicy]`` - *(optional)* Resources resize policy for the container.
       * **resources** ``ResourceRequirements`` - *(optional)* Compute Resources required by this container. Cannot be updated. More info:
         https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/
       * **securityContext** ``SecurityContext`` - *(optional)* SecurityContext defines the security options the container should be run with.
         If set, the fields of SecurityContext override the equivalent fields of
         PodSecurityContext. More info:
         https://kubernetes.io/docs/tasks/configure-pod-container/security-context/
       * **startupProbe** ``Probe`` - *(optional)* StartupProbe indicates that the Pod has successfully initialized. If
@@ -777,14 +777,15 @@
     envFrom: 'List[EnvFromSource]' = None
     image: 'str' = None
     imagePullPolicy: 'str' = None
     lifecycle: 'Lifecycle' = None
     livenessProbe: 'Probe' = None
     ports: 'List[ContainerPort]' = None
     readinessProbe: 'Probe' = None
+    resizePolicy: 'List[ContainerResizePolicy]' = None
     resources: 'ResourceRequirements' = None
     securityContext: 'SecurityContext' = None
     startupProbe: 'Probe' = None
     stdin: 'bool' = None
     stdinOnce: 'bool' = None
     terminationMessagePath: 'str' = None
     terminationMessagePolicy: 'str' = None
@@ -830,14 +831,29 @@
     hostIP: 'str' = None
     hostPort: 'int' = None
     name: 'str' = None
     protocol: 'str' = None
 
 
 @dataclass
+class ContainerResizePolicy(DataclassDictMixIn):
+    """ContainerResizePolicy represents resource resize policy for the container.
+
+      **parameters**
+
+      * **resourceName** ``str`` - Name of the resource to which this resource resize policy applies. Supported
+        values: cpu, memory.
+      * **restartPolicy** ``str`` - Restart policy to apply when specified resource is resized. If not specified,
+        it defaults to NotRequired.
+    """
+    resourceName: 'str'
+    restartPolicy: 'str'
+
+
+@dataclass
 class ContainerState(DataclassDictMixIn):
     """ContainerState holds a possible state of container. Only one of its members
       may be specified. If none of them is specified, the default one is
       ContainerStateWaiting.
 
       **parameters**
 
@@ -899,36 +915,65 @@
 
 @dataclass
 class ContainerStatus(DataclassDictMixIn):
     """ContainerStatus contains details for the current status of this container.
 
       **parameters**
 
-      * **image** ``str`` - The image the container is running. More info:
+      * **image** ``str`` - Image is the name of container image that the container is running. The
+        container image may not match the image used in the PodSpec, as it may have
+        been resolved by the runtime. More info:
         https://kubernetes.io/docs/concepts/containers/images.
-      * **imageID** ``str`` - ImageID of the container's image.
-      * **name** ``str`` - This must be a DNS_LABEL. Each container in a pod must have a unique name.
-        Cannot be updated.
-      * **ready** ``bool`` - Specifies whether the container has passed its readiness probe.
-      * **restartCount** ``int`` - The number of times the container has been restarted.
-      * **containerID** ``str`` - *(optional)* Container's ID in the format '<type>://<container_id>'.
-      * **lastState** ``ContainerState`` - *(optional)* Details about the container's last termination condition.
-      * **started** ``bool`` - *(optional)* Specifies whether the container has passed its startup probe. Initialized as
-        false, becomes true after startupProbe is considered successful. Resets to
-        false when the container is restarted, or if kubelet loses state temporarily.
-        Is always true when no startupProbe is defined.
-      * **state** ``ContainerState`` - *(optional)* Details about the container's current condition.
+      * **imageID** ``str`` - ImageID is the image ID of the container's image. The image ID may not match
+        the image ID of the image used in the PodSpec, as it may have been resolved by
+        the runtime.
+      * **name** ``str`` - Name is a DNS_LABEL representing the unique name of the container. Each
+        container in a pod must have a unique name across all container types. Cannot
+        be updated.
+      * **ready** ``bool`` - Ready specifies whether the container is currently passing its readiness
+        check. The value will change as readiness probes keep executing. If no
+        readiness probes are specified, this field defaults to true once the container
+        is fully started (see Started field).
+        The value is typically used to determine whether a container is ready to
+        accept traffic.
+      * **restartCount** ``int`` - RestartCount holds the number of times the container has been restarted.
+        Kubelet makes an effort to always increment the value, but there are cases
+        when the state may be lost due to node restarts and then the value may be
+        reset to 0. The value is never negative.
+      * **allocatedResources** ``dict`` - *(optional)* AllocatedResources represents the compute resources allocated for this
+        container by the node. Kubelet sets this value to Container.Resources.Requests
+        upon successful pod admission and after successfully admitting desired pod
+        resize.
+      * **containerID** ``str`` - *(optional)* ContainerID is the ID of the container in the format
+        '<type>://<container_id>'. Where type is a container runtime identifier,
+        returned from Version call of CRI API (for example "containerd").
+      * **lastState** ``ContainerState`` - *(optional)* LastTerminationState holds the last termination state of the container to help
+        debug container crashes and restarts. This field is not populated if the
+        container is still running and RestartCount is 0.
+      * **resources** ``ResourceRequirements`` - *(optional)* Resources represents the compute resource requests and limits that have been
+        successfully enacted on the running container after it has been started or has
+        been successfully resized.
+      * **started** ``bool`` - *(optional)* Started indicates whether the container has finished its postStart lifecycle
+        hook and passed its startup probe. Initialized as false, becomes true after
+        startupProbe is considered successful. Resets to false when the container is
+        restarted, or if kubelet loses state temporarily. In both cases, startup
+        probes will run again. Is always true when no startupProbe is defined and
+        container is running and has passed the postStart lifecycle hook. The null
+        value must be treated the same as false.
+      * **state** ``ContainerState`` - *(optional)* State holds details about the container's current condition.
     """
     image: 'str'
     imageID: 'str'
     name: 'str'
     ready: 'bool'
     restartCount: 'int'
+    allocatedResources: 'dict' = None
     containerID: 'str' = None
     lastState: 'ContainerState' = None
+    resources: 'ResourceRequirements' = None
     started: 'bool' = None
     state: 'ContainerState' = None
 
 
 @dataclass
 class DaemonEndpoint(DataclassDictMixIn):
     """DaemonEndpoint contains information about a single Daemon endpoint.
@@ -1012,30 +1057,29 @@
         string (default) or Memory. More info:
         https://kubernetes.io/docs/concepts/storage/volumes#emptydir
       * **sizeLimit** ``resource.Quantity`` - *(optional)* sizeLimit is the total amount of local storage required for this EmptyDir
         volume. The size limit is also applicable for memory medium. The maximum usage
         on memory medium EmptyDir would be the minimum value between the SizeLimit
         specified here and the sum of memory limits of all containers in a pod. The
         default is nil which means that the limit is undefined. More info:
-        http://kubernetes.io/docs/user-guide/volumes#emptydir
+        https://kubernetes.io/docs/concepts/storage/volumes#emptydir
     """
     medium: 'str' = None
     sizeLimit: 'resource.Quantity' = None
 
 
 @dataclass
 class EndpointAddress(DataclassDictMixIn):
     """EndpointAddress is a tuple that describes single IP address.
 
       **parameters**
 
-      * **ip** ``str`` - The IP of this endpoint. May not be loopback (127.0.0.0/8), link-local
-        (169.254.0.0/16), or link-local multicast ((224.0.0.0/24). IPv6 is also
-        accepted but not fully supported on all platforms. Also, certain kubernetes
-        components, like kube-proxy, are not IPv6 ready.
+      * **ip** ``str`` - The IP of this endpoint. May not be loopback (127.0.0.0/8 or ::1), link-local
+        (169.254.0.0/16 or fe80::/10), or link-local multicast (224.0.0.0/24 or
+        ff02::/16).
       * **hostname** ``str`` - *(optional)* The Hostname of this endpoint
       * **nodeName** ``str`` - *(optional)* Optional: Node hosting this endpoint. This can be used to determine endpoints
         local to a node.
       * **targetRef** ``ObjectReference`` - *(optional)* Reference to object providing the endpoint.
     """
     ip: 'str'
     hostname: 'str' = None
@@ -1046,18 +1090,23 @@
 @dataclass
 class EndpointPort(DataclassDictMixIn):
     """EndpointPort is a tuple that describes a single port.
 
       **parameters**
 
       * **port** ``int`` - The port number of the endpoint.
-      * **appProtocol** ``str`` - *(optional)* The application protocol for this port. This field follows standard Kubernetes
-        label syntax. Un-prefixed names are reserved for IANA standard service names
-        (as per RFC-6335 and https://www.iana.org/assignments/service-names).
-        Non-standard protocols should use prefixed names such as
+      * **appProtocol** ``str`` - *(optional)* The application protocol for this port. This is used as a hint for
+        implementations to offer richer behavior for protocols that they understand.
+        This field follows standard Kubernetes label syntax. Valid values are either:
+        * Un-prefixed protocol names - reserved for IANA standard service names (as
+        per RFC-6335 and https://www.iana.org/assignments/service-names).
+        * Kubernetes-defined prefixed names:
+          * 'kubernetes.io/h2c' - HTTP/2 over cleartext as described in
+        https://www.rfc-editor.org/rfc/rfc7540
+        * Other protocols should use implementation-defined prefixed names such as
         mycompany.com/my-custom-protocol.
       * **name** ``str`` - *(optional)* The name of this port.  This must match the 'name' field in the corresponding
         ServicePort. Must be a DNS_LABEL. Optional only if one port is defined.
       * **protocol** ``str`` - *(optional)* The IP protocol for this port. Must be UDP, TCP, or SCTP. Default is TCP.
     """
     port: 'int'
     appProtocol: 'str' = None
@@ -1266,14 +1315,15 @@
       * **imagePullPolicy** ``str`` - *(optional)* Image pull policy. One of Always, Never, IfNotPresent. Defaults to Always if
         :latest tag is specified, or IfNotPresent otherwise. Cannot be updated. More
         info: https://kubernetes.io/docs/concepts/containers/images#updating-images
       * **lifecycle** ``Lifecycle`` - *(optional)* Lifecycle is not allowed for ephemeral containers.
       * **livenessProbe** ``Probe`` - *(optional)* Probes are not allowed for ephemeral containers.
       * **ports** ``List[ContainerPort]`` - *(optional)* Ports are not allowed for ephemeral containers.
       * **readinessProbe** ``Probe`` - *(optional)* Probes are not allowed for ephemeral containers.
+      * **resizePolicy** ``List[ContainerResizePolicy]`` - *(optional)* Resources resize policy for the container.
       * **resources** ``ResourceRequirements`` - *(optional)* Resources are not allowed for ephemeral containers. Ephemeral containers use
         spare resources already allocated to the pod.
       * **securityContext** ``SecurityContext`` - *(optional)* Optional: SecurityContext defines the security options the ephemeral container
         should be run with. If set, the fields of SecurityContext override the
         equivalent fields of PodSecurityContext.
       * **startupProbe** ``Probe`` - *(optional)* Probes are not allowed for ephemeral containers.
       * **stdin** ``bool`` - *(optional)* Whether this container should allocate a buffer for stdin in the container
@@ -1322,14 +1372,15 @@
     envFrom: 'List[EnvFromSource]' = None
     image: 'str' = None
     imagePullPolicy: 'str' = None
     lifecycle: 'Lifecycle' = None
     livenessProbe: 'Probe' = None
     ports: 'List[ContainerPort]' = None
     readinessProbe: 'Probe' = None
+    resizePolicy: 'List[ContainerResizePolicy]' = None
     resources: 'ResourceRequirements' = None
     securityContext: 'SecurityContext' = None
     startupProbe: 'Probe' = None
     stdin: 'bool' = None
     stdinOnce: 'bool' = None
     targetContainerName: 'str' = None
     terminationMessagePath: 'str' = None
@@ -2468,15 +2519,19 @@
       **parameters**
 
       * **addresses** ``List[NodeAddress]`` - *(optional)* List of addresses reachable to the node. Queried from cloud provider, if
         available. More info:
         https://kubernetes.io/docs/concepts/nodes/node/#addresses Note: This field is
         declared as mergeable, but the merge key is not sufficiently unique, which can
         cause data corruption when it is merged. Callers should instead use a
-        full-replacement patch. See https://pr.k8s.io/79391 for an example.
+        full-replacement patch. See https://pr.k8s.io/79391 for an example. Consumers
+        should assume that addresses can change during the lifetime of a Node.
+        However, there are some exceptions where this may not be possible, such as
+        Pods that inherit a Node's address in its own status or consumers of the
+        downward API (status.hostIP).
       * **allocatable** ``dict`` - *(optional)* Allocatable represents the resources of a node that are available for
         scheduling. Defaults to Capacity.
       * **capacity** ``dict`` - *(optional)* Capacity represents the total resources of a node. More info:
         https://kubernetes.io/docs/concepts/storage/persistent-volumes#capacity
       * **conditions** ``List[NodeCondition]`` - *(optional)* Conditions is an array of current observed node conditions. More info:
         https://kubernetes.io/docs/concepts/nodes/node/#condition
       * **config** ``NodeConfigStatus`` - *(optional)* Status of the config assigned to the node via the dynamic Kubelet config
@@ -2649,15 +2704,15 @@
     metadata: 'meta_v1.ObjectMeta' = None
     spec: 'PersistentVolumeClaimSpec' = None
     status: 'PersistentVolumeClaimStatus' = None
 
 
 @dataclass
 class PersistentVolumeClaimCondition(DataclassDictMixIn):
-    """PersistentVolumeClaimCondition contails details about state of pvc
+    """PersistentVolumeClaimCondition contains details about state of pvc
 
       **parameters**
 
       * **status** ``str`` - 
       * **type** ``str`` - 
       * **lastProbeTime** ``meta_v1.Time`` - *(optional)* lastProbeTime is the time we probed the condition.
       * **lastTransitionTime** ``meta_v1.Time`` - *(optional)* lastTransitionTime is the time the condition transitioned from one status to
@@ -3479,28 +3534,31 @@
       * **resourceClaims** ``List[PodResourceClaim]`` - *(optional)* ResourceClaims defines which ResourceClaims must be allocated and reserved
         before the Pod is allowed to start. The resources will be made available to
         those containers which consume them by name.
         This is an alpha field and requires enabling the DynamicResourceAllocation
         feature gate.
         This field is immutable.
       * **restartPolicy** ``str`` - *(optional)* Restart policy for all containers within the pod. One of Always, OnFailure,
-        Never. Default to Always. More info:
+        Never. In some contexts, only a subset of those values may be permitted.
+        Default to Always. More info:
         https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle/#restart-policy
       * **runtimeClassName** ``str`` - *(optional)* RuntimeClassName refers to a RuntimeClass object in the node.k8s.io group,
         which should be used to run this pod.  If no RuntimeClass resource matches the
         named class, the pod will not be run. If unset or empty, the "legacy"
         RuntimeClass will be used, which is an implicit class with an empty definition
         that uses the default runtime handler. More info:
         https://git.k8s.io/enhancements/keps/sig-node/585-runtime-class
       * **schedulerName** ``str`` - *(optional)* If specified, the pod will be dispatched by specified scheduler. If not
         specified, the pod will be dispatched by default scheduler.
       * **schedulingGates** ``List[PodSchedulingGate]`` - *(optional)* SchedulingGates is an opaque list of values that if specified will block
-        scheduling the pod. More info:
-        https://git.k8s.io/enhancements/keps/sig-scheduling/3521-pod-scheduling-readiness.
-        This is an alpha-level feature enabled by PodSchedulingReadiness feature gate.
+        scheduling the pod. If schedulingGates is not empty, the pod will stay in the
+        SchedulingGated state and the scheduler will not attempt to schedule the pod.
+        SchedulingGates can only be set at pod creation time, and be removed only
+        afterwards.
+        This is a beta feature enabled by the PodSchedulingReadiness feature gate.
       * **securityContext** ``PodSecurityContext`` - *(optional)* SecurityContext holds pod-level security attributes and common container
         settings. Optional: Defaults to empty.  See type description for default
         values of each field.
       * **serviceAccount** ``str`` - *(optional)* DeprecatedServiceAccount is a depreciated alias for ServiceAccountName.
         Deprecated: Use serviceAccountName instead.
       * **serviceAccountName** ``str`` - *(optional)* ServiceAccountName is the name of the ServiceAccount to use to run this pod.
         More info:
@@ -3627,17 +3685,20 @@
       * **podIPs** ``List[PodIP]`` - *(optional)* podIPs holds the IP addresses allocated to the pod. If this field is
         specified, the 0th entry must match the podIP field. Pods may be allocated at
         most 1 value for each of IPv4 and IPv6. This list is empty if no IPs have been
         allocated yet.
       * **qosClass** ``str`` - *(optional)* The Quality of Service (QOS) classification assigned to the pod based on
         resource requirements See PodQOSClass type for available QOS classes More
         info:
-        https://git.k8s.io/community/contributors/design-proposals/node/resource-qos.md
+        https://kubernetes.io/docs/concepts/workloads/pods/pod-qos/#quality-of-service-classes
       * **reason** ``str`` - *(optional)* A brief CamelCase message indicating details about why the pod is in this
         state. e.g. 'Evicted'
+      * **resize** ``str`` - *(optional)* Status of resources resize desired for pod's containers. It is empty if no
+        resources resize is pending. Any changes to container resources will
+        automatically set this to "Proposed"
       * **startTime** ``meta_v1.Time`` - *(optional)* RFC 3339 date and time at which the object was acknowledged by the Kubelet.
         This is before the Kubelet pulled the container image(s) for the pod.
     """
     conditions: 'List[PodCondition]' = None
     containerStatuses: 'List[ContainerStatus]' = None
     ephemeralContainerStatuses: 'List[ContainerStatus]' = None
     hostIP: 'str' = None
@@ -3645,14 +3706,15 @@
     message: 'str' = None
     nominatedNodeName: 'str' = None
     phase: 'str' = None
     podIP: 'str' = None
     podIPs: 'List[PodIP]' = None
     qosClass: 'str' = None
     reason: 'str' = None
+    resize: 'str' = None
     startTime: 'meta_v1.Time' = None
 
 
 @dataclass
 class PodTemplate(DataclassDictMixIn):
     """PodTemplate describes a template for creating copies of a predefined pod.
 
@@ -3778,16 +3840,15 @@
       determine whether it is alive or ready to receive traffic.
 
       **parameters**
 
       * **exec** ``ExecAction`` - *(optional)* Exec specifies the action to take.
       * **failureThreshold** ``int`` - *(optional)* Minimum consecutive failures for the probe to be considered failed after
         having succeeded. Defaults to 3. Minimum value is 1.
-      * **grpc** ``GRPCAction`` - *(optional)* GRPC specifies an action involving a GRPC port. This is a beta field and
-        requires enabling GRPCContainerProbe feature gate.
+      * **grpc** ``GRPCAction`` - *(optional)* GRPC specifies an action involving a GRPC port.
       * **httpGet** ``HTTPGetAction`` - *(optional)* HTTPGet specifies the http request to perform.
       * **initialDelaySeconds** ``int`` - *(optional)* Number of seconds after the container has started before liveness probes are
         initiated. More info:
         https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes
       * **periodSeconds** ``int`` - *(optional)* How often (in seconds) to perform the probe. Default to 10 seconds. Minimum
         value is 1.
       * **successThreshold** ``int`` - *(optional)* Minimum consecutive successes for the probe to be considered successful after
@@ -4036,15 +4097,15 @@
         Selector is empty, it is defaulted to the labels present on the Pod template.
         Label keys and values that must match in order to be controlled by this
         replication controller, if empty defaulted to labels on Pod template. More
         info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors
       * **template** ``PodTemplateSpec`` - *(optional)* Template is the object that describes the pod that will be created if
         insufficient replicas are detected. This takes precedence over a TemplateRef.
-        More info:
+        The only allowed template.spec.restartPolicy value is "Always". More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller#pod-template
     """
     minReadySeconds: 'int' = None
     replicas: 'int' = None
     selector: 'dict' = None
     template: 'PodTemplateSpec' = None
 
@@ -4197,20 +4258,21 @@
 
       **parameters**
 
       * **claims** ``List[ResourceClaim]`` - *(optional)* Claims lists the names of resources, defined in spec.resourceClaims, that are
         used by this container.
         This is an alpha field and requires enabling the DynamicResourceAllocation
         feature gate.
-        This field is immutable.
+        This field is immutable. It can only be set for containers.
       * **limits** ``dict`` - *(optional)* Limits describes the maximum amount of compute resources allowed. More info:
         https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/
       * **requests** ``dict`` - *(optional)* Requests describes the minimum amount of compute resources required. If
         Requests is omitted for a container, it defaults to Limits if that is
-        explicitly specified, otherwise to an implementation-defined value. More info:
+        explicitly specified, otherwise to an implementation-defined value. Requests
+        cannot exceed Limits. More info:
         https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/
     """
     claims: 'List[ResourceClaim]' = None
     limits: 'dict' = None
     requests: 'dict' = None
 
 
@@ -5221,16 +5283,20 @@
       * **labelSelector** ``meta_v1.LabelSelector`` - *(optional)* LabelSelector is used to find matching pods. Pods that match this label
         selector are counted to determine the number of pods in their corresponding
         topology domain.
       * **matchLabelKeys** ``List[str]`` - *(optional)* MatchLabelKeys is a set of pod label keys to select the pods over which
         spreading will be calculated. The keys are used to lookup values from the
         incoming pod labels, those key-value labels are ANDed with labelSelector to
         select the group of existing pods over which spreading will be calculated for
-        the incoming pod. Keys that don't exist in the incoming pod labels will be
-        ignored. A null or empty list means only match against labelSelector.
+        the incoming pod. The same key is forbidden to exist in both MatchLabelKeys
+        and LabelSelector. MatchLabelKeys cannot be set when LabelSelector isn't set.
+        Keys that don't exist in the incoming pod labels will be ignored. A null or
+        empty list means only match against labelSelector.
+        This is a beta field and requires the MatchLabelKeysInPodTopologySpread
+        feature gate to be enabled (enabled by default).
       * **minDomains** ``int`` - *(optional)* MinDomains indicates a minimum number of eligible domains. When the number of
         eligible domains with matching topology keys is less than minDomains, Pod
         Topology Spread treats "global minimum" as 0, and then the calculation of Skew
         is performed. And when the number of eligible domains with matching topology
         keys equals or greater than minDomains, this value has no effect on
         scheduling. As a result, when the number of eligible domains is less than
         minDomains, scheduler won't schedule more than maxSkew Pods to those domains.
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/discovery_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/discovery_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from . import meta_v1
 from . import core_v1
+from . import meta_v1
 
 
 @dataclass
 class Endpoint(DataclassDictMixIn):
     """Endpoint represents a single logical "backend" implementing a service.
 
       **parameters**
@@ -53,15 +53,17 @@
 
       **parameters**
 
       * **ready** ``bool`` - *(optional)* ready indicates that this endpoint is prepared to receive traffic, according
         to whatever system is managing the endpoint. A nil value indicates an unknown
         state. In most cases consumers should interpret this unknown state as ready.
         For compatibility reasons, ready should never be "true" for terminating
-        endpoints.
+        endpoints, except when the normal readiness behavior is being explicitly
+        overridden, for example when the associated Service has set the
+        publishNotReadyAddresses flag.
       * **serving** ``bool`` - *(optional)* serving is identical to ready except that it is set regardless of the
         terminating state of endpoints. This condition should be set to true for a
         ready endpoint that is terminating. If nil, consumers should defer to the
         ready condition.
       * **terminating** ``bool`` - *(optional)* terminating indicates that this endpoint is terminating. A nil value indicates
         an unknown state. Consumers should interpret this unknown state to mean that
         the endpoint is not terminating.
@@ -85,28 +87,35 @@
 
 @dataclass
 class EndpointPort(DataclassDictMixIn):
     """EndpointPort represents a Port used by an EndpointSlice
 
       **parameters**
 
-      * **appProtocol** ``str`` - *(optional)* The application protocol for this port. This field follows standard Kubernetes
-        label syntax. Un-prefixed names are reserved for IANA standard service names
-        (as per RFC-6335 and https://www.iana.org/assignments/service-names).
-        Non-standard protocols should use prefixed names such as
+      * **appProtocol** ``str`` - *(optional)* The application protocol for this port. This is used as a hint for
+        implementations to offer richer behavior for protocols that they understand.
+        This field follows standard Kubernetes label syntax. Valid values are either:
+        * Un-prefixed protocol names - reserved for IANA standard service names (as
+        per RFC-6335 and https://www.iana.org/assignments/service-names).
+        * Kubernetes-defined prefixed names:
+          * 'kubernetes.io/h2c' - HTTP/2 over cleartext as described in
+        https://www.rfc-editor.org/rfc/rfc7540
+        * Other protocols should use implementation-defined prefixed names such as
         mycompany.com/my-custom-protocol.
-      * **name** ``str`` - *(optional)* The name of this port. All ports in an EndpointSlice must have a unique name.
-        If the EndpointSlice is dervied from a Kubernetes service, this corresponds to
-        the Service.ports[].name. Name must either be an empty string or pass
-        DNS_LABEL validation: * must be no more than 63 characters long. * must
-        consist of lower case alphanumeric characters or '-'. * must start and end
-        with an alphanumeric character. Default is empty string.
-      * **port** ``int`` - *(optional)* The port number of the endpoint. If this is not specified, ports are not
-        restricted and must be interpreted in the context of the specific consumer.
-      * **protocol** ``str`` - *(optional)* The IP protocol for this port. Must be UDP, TCP, or SCTP. Default is TCP.
+      * **name** ``str`` - *(optional)* name represents the name of this port. All ports in an EndpointSlice must have
+        a unique name. If the EndpointSlice is dervied from a Kubernetes service, this
+        corresponds to the Service.ports[].name. Name must either be an empty string
+        or pass DNS_LABEL validation: * must be no more than 63 characters long. *
+        must consist of lower case alphanumeric characters or '-'. * must start and
+        end with an alphanumeric character. Default is empty string.
+      * **port** ``int`` - *(optional)* port represents the port number of the endpoint. If this is not specified,
+        ports are not restricted and must be interpreted in the context of the
+        specific consumer.
+      * **protocol** ``str`` - *(optional)* protocol represents the IP protocol for this port. Must be UDP, TCP, or SCTP.
+        Default is TCP.
     """
     appProtocol: 'str' = None
     name: 'str' = None
     port: 'int' = None
     protocol: 'str' = None
 
 
@@ -149,15 +158,15 @@
 
 @dataclass
 class EndpointSliceList(DataclassDictMixIn):
     """EndpointSliceList represents a list of endpoint slices
 
       **parameters**
 
-      * **items** ``List[EndpointSlice]`` - List of endpoint slices
+      * **items** ``List[EndpointSlice]`` - items is the list of endpoint slices
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/events_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/events_v1.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from . import core_v1
 from . import meta_v1
+from . import core_v1
 
 
 @dataclass
 class Event(DataclassDictMixIn):
     """Event is a report of an event somewhere in the cluster. It generally denotes
       some state change in the system. Events have a limited retention time and
       triggers and messages may evolve with time.  Event consumers should not rely
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/flowcontrol_v1beta2.py` & `lightkube-models-1.27.1.4/lightkube/models/flowcontrol_v1beta2.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/models/flowcontrol_v1beta3.py` & `lightkube-models-1.27.1.4/lightkube/models/flowcontrol_v1beta3.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/models/meta_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/meta_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from datetime import datetime
 from . import runtime
+from datetime import datetime
 from typing import Dict
 
 
 @dataclass
 class APIGroup(DataclassDictMixIn):
     """APIGroup contains the name, the supported versions, and the preferred version
       of a group.
@@ -392,15 +392,15 @@
       all objects users must create.
 
       **parameters**
 
       * **annotations** ``dict`` - *(optional)* Annotations is an unstructured key value map stored with a resource that may
         be set by external tools to store and retrieve arbitrary metadata. They are
         not queryable and should be preserved when modifying objects. More info:
-        http://kubernetes.io/docs/user-guide/annotations
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
       * **creationTimestamp** ``Time`` - *(optional)* CreationTimestamp is a timestamp representing the server time when this object
         was created. It is not guaranteed to be set in happens-before order across
         separate operations. Clients may not set this value. It is represented in
         RFC3339 form and is in UTC.
         Populated by the system. Read-only. Null for lists. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
       * **deletionGracePeriodSeconds** ``int`` - *(optional)* Number of seconds allowed for this object to gracefully terminate before it
@@ -448,32 +448,33 @@
         return a 409.
         Applied only if Name is not specified. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency
       * **generation** ``int`` - *(optional)* A sequence number representing a specific generation of the desired state.
         Populated by the system. Read-only.
       * **labels** ``dict`` - *(optional)* Map of string keys and values that can be used to organize and categorize
         (scope and select) objects. May match selectors of replication controllers and
-        services. More info: http://kubernetes.io/docs/user-guide/labels
+        services. More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/labels
       * **managedFields** ``List[ManagedFieldsEntry]`` - *(optional)* ManagedFields maps workflow-id and version to the set of fields that are
         managed by that workflow. This is mostly for internal housekeeping, and users
         typically shouldn't need to set or understand this field. A workflow can be
         the user's name, a controller's name, or the name of a specific apply path
         like "ci-cd". The set of fields is always in the version that the workflow
         used when modifying the object.
       * **name** ``str`` - *(optional)* Name must be unique within a namespace. Is required when creating resources,
         although some resources may allow a client to request the generation of an
         appropriate name automatically. Name is primarily intended for creation
         idempotence and configuration definition. Cannot be updated. More info:
-        http://kubernetes.io/docs/user-guide/identifiers#names
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names
       * **namespace** ``str`` - *(optional)* Namespace defines the space within which each name must be unique. An empty
         namespace is equivalent to the "default" namespace, but "default" is the
         canonical representation. Not all objects are required to be scoped to a
         namespace - the value of this field for those objects will be empty.
         Must be a DNS_LABEL. Cannot be updated. More info:
-        http://kubernetes.io/docs/user-guide/namespaces
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces
       * **ownerReferences** ``List[OwnerReference]`` - *(optional)* List of objects depended by this object. If ALL objects in the list have been
         deleted, this object will be garbage collected. If this object is managed by a
         controller, then an entry in this list will point to this controller, with the
         controller field set to true. There cannot be more than one managing
         controller.
       * **resourceVersion** ``str`` - *(optional)* An opaque value that represents the internal version of this object that can
         be used by clients to determine when objects have changed. May be used for
@@ -486,15 +487,15 @@
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency
       * **selfLink** ``str`` - *(optional)* Deprecated: selfLink is a legacy read-only field that is no longer populated
         by the system.
       * **uid** ``str`` - *(optional)* UID is the unique in time and space value for this object. It is typically
         generated by the server on successful creation of a resource and is not
         allowed to change on PUT operations.
         Populated by the system. Read-only. More info:
-        http://kubernetes.io/docs/user-guide/identifiers#uids
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids
     """
     annotations: 'dict' = None
     creationTimestamp: 'Time' = None
     deletionGracePeriodSeconds: 'int' = None
     deletionTimestamp: 'Time' = None
     finalizers: 'List[str]' = None
     generateName: 'str' = None
@@ -517,17 +518,17 @@
 
       **parameters**
 
       * **apiVersion** ``str`` - API version of the referent.
       * **kind** ``str`` - Kind of the referent. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **name** ``str`` - Name of the referent. More info:
-        http://kubernetes.io/docs/user-guide/identifiers#names
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names
       * **uid** ``str`` - UID of the referent. More info:
-        http://kubernetes.io/docs/user-guide/identifiers#uids
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids
       * **blockOwnerDeletion** ``bool`` - *(optional)* If true, AND if the owner has the "foregroundDeletion" finalizer, then the
         owner cannot be deleted from the key-value store until this reference is
         removed. See
         https://kubernetes.io/docs/concepts/architecture/garbage-collection/#foreground-deletion
         for how the garbage collector interacts with this field and enforces the
         foreground deletion. Defaults to false. To set this field, a user needs
         "delete" permission of the owner, otherwise 422 (Unprocessable Entity) will be
@@ -655,15 +656,16 @@
       * **name** ``str`` - *(optional)* The name attribute of the resource associated with the status StatusReason
         (when there is a single name which can be described).
       * **retryAfterSeconds** ``int`` - *(optional)* If specified, the time in seconds before the operation should be retried. Some
         errors may indicate the client must take an alternate action - for those
         errors this field may indicate how long to wait before taking the alternate
         action.
       * **uid** ``str`` - *(optional)* UID of the resource. (when there is a single resource which can be described).
-        More info: http://kubernetes.io/docs/user-guide/identifiers#uids
+        More info:
+        https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids
     """
     causes: 'List[StatusCause]' = None
     group: 'str' = None
     kind: 'str' = None
     name: 'str' = None
     retryAfterSeconds: 'int' = None
     uid: 'str' = None
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/networking_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/networking_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 @dataclass
 class HTTPIngressPath(DataclassDictMixIn):
     """HTTPIngressPath associates a path with a backend. Incoming urls matching the
       path are forwarded to the backend.
 
       **parameters**
 
-      * **backend** ``IngressBackend`` - Backend defines the referenced service endpoint to which the traffic will be
+      * **backend** ``IngressBackend`` - backend defines the referenced service endpoint to which the traffic will be
         forwarded to.
-      * **pathType** ``str`` - PathType determines the interpretation of the Path matching. PathType can be
+      * **pathType** ``str`` - pathType determines the interpretation of the path matching. PathType can be
         one of the following values: * Exact: Matches the URL path exactly. * Prefix:
         Matches based on a URL path prefix split by '/'. Matching is
           done on a path element by element basis. A path element refers is the
           list of labels in the path split by the '/' separator. A request is a
           match for path p if every p is an element-wise prefix of p of the
           request path. Note that if the last element of the path is a substring
           of the last element in request path, it is not a match (e.g. /foo/bar
           matches /foo/bar/baz, but does not match /foo/barbaz).
         * ImplementationSpecific: Interpretation of the Path matching is up to
           the IngressClass. Implementations can treat this as a separate PathType
           or treat it identically to Prefix or Exact path types.
         Implementations are required to support all path types.
-      * **path** ``str`` - *(optional)* Path is matched against the path of an incoming request. Currently it can
+      * **path** ``str`` - *(optional)* path is matched against the path of an incoming request. Currently it can
         contain characters disallowed from the conventional "path" part of a URL as
         defined by RFC 3986. Paths must begin with a '/' and must be present when
         using PathType with value "Exact" or "Prefix".
     """
     backend: 'IngressBackend'
     pathType: 'str'
     path: 'str' = None
@@ -46,32 +46,32 @@
     """HTTPIngressRuleValue is a list of http selectors pointing to backends. In the
       example: http://<host>/<path>?<searchpart> -> backend where where parts of the
       url correspond to RFC 3986, this resource will be used to match against
       everything after the last '/' and before the first '?' or '#'.
 
       **parameters**
 
-      * **paths** ``List[HTTPIngressPath]`` - A collection of paths that map requests to backends.
+      * **paths** ``List[HTTPIngressPath]`` - paths is a collection of paths that map requests to backends.
     """
     paths: 'List[HTTPIngressPath]'
 
 
 @dataclass
 class IPBlock(DataclassDictMixIn):
     """IPBlock describes a particular CIDR (Ex. "192.168.1.0/24","2001:db8::/64")
       that is allowed to the pods matched by a NetworkPolicySpec's podSelector. The
       except entry describes CIDRs that should not be included within this rule.
 
       **parameters**
 
-      * **cidr** ``str`` - CIDR is a string representing the IP Block Valid examples are "192.168.1.0/24"
+      * **cidr** ``str`` - cidr is a string representing the IPBlock Valid examples are "192.168.1.0/24"
         or "2001:db8::/64"
-      * **except_** ``List[str]`` - *(optional)* Except is a slice of CIDRs that should not be included within an IP Block
-        Valid examples are "192.168.1.0/24" or "2001:db8::/64" Except values will be
-        rejected if they are outside the CIDR range
+      * **except_** ``List[str]`` - *(optional)* except is a slice of CIDRs that should not be included within an IPBlock Valid
+        examples are "192.168.1.0/24" or "2001:db8::/64" Except values will be
+        rejected if they are outside the cidr range
     """
     cidr: 'str'
     except_: 'List[str]' = field(metadata={"json": "except"}, default=None)
 
 
 @dataclass
 class Ingress(DataclassDictMixIn):
@@ -88,17 +88,17 @@
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object's metadata. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **spec** ``IngressSpec`` - *(optional)* Spec is the desired state of the Ingress. More info:
+      * **spec** ``IngressSpec`` - *(optional)* spec is the desired state of the Ingress. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status
-      * **status** ``IngressStatus`` - *(optional)* Status is the current state of the Ingress. More info:
+      * **status** ``IngressStatus`` - *(optional)* status is the current state of the Ingress. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status
     """
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
     spec: 'IngressSpec' = None
     status: 'IngressStatus' = None
@@ -106,18 +106,18 @@
 
 @dataclass
 class IngressBackend(DataclassDictMixIn):
     """IngressBackend describes all endpoints for a given service and port.
 
       **parameters**
 
-      * **resource** ``core_v1.TypedLocalObjectReference`` - *(optional)* Resource is an ObjectRef to another Kubernetes resource in the namespace of
+      * **resource** ``core_v1.TypedLocalObjectReference`` - *(optional)* resource is an ObjectRef to another Kubernetes resource in the namespace of
         the Ingress object. If resource is specified, a service.Name and service.Port
         must not be specified. This is a mutually exclusive setting with "Service".
-      * **service** ``IngressServiceBackend`` - *(optional)* Service references a Service as a Backend. This is a mutually exclusive
+      * **service** ``IngressServiceBackend`` - *(optional)* service references a service as a backend. This is a mutually exclusive
         setting with "Resource".
     """
     resource: 'core_v1.TypedLocalObjectReference' = None
     service: 'IngressServiceBackend' = None
 
 
 @dataclass
@@ -136,30 +136,30 @@
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object's metadata. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **spec** ``IngressClassSpec`` - *(optional)* Spec is the desired state of the IngressClass. More info:
+      * **spec** ``IngressClassSpec`` - *(optional)* spec is the desired state of the IngressClass. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status
     """
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
     spec: 'IngressClassSpec' = None
 
 
 @dataclass
 class IngressClassList(DataclassDictMixIn):
     """IngressClassList is a collection of IngressClasses.
 
       **parameters**
 
-      * **items** ``List[IngressClass]`` - Items is the list of IngressClasses.
+      * **items** ``List[IngressClass]`` - items is the list of IngressClasses.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
@@ -175,23 +175,23 @@
 @dataclass
 class IngressClassParametersReference(DataclassDictMixIn):
     """IngressClassParametersReference identifies an API object. This can be used to
       specify a cluster or namespace-scoped resource.
 
       **parameters**
 
-      * **kind** ``str`` - Kind is the type of resource being referenced.
-      * **name** ``str`` - Name is the name of resource being referenced.
-      * **apiGroup** ``str`` - *(optional)* APIGroup is the group for the resource being referenced. If APIGroup is not
+      * **kind** ``str`` - kind is the type of resource being referenced.
+      * **name** ``str`` - name is the name of resource being referenced.
+      * **apiGroup** ``str`` - *(optional)* apiGroup is the group for the resource being referenced. If APIGroup is not
         specified, the specified Kind must be in the core API group. For any other
         third-party types, APIGroup is required.
-      * **namespace** ``str`` - *(optional)* Namespace is the namespace of the resource being referenced. This field is
+      * **namespace** ``str`` - *(optional)* namespace is the namespace of the resource being referenced. This field is
         required when scope is set to "Namespace" and must be unset when scope is set
         to "Cluster".
-      * **scope** ``str`` - *(optional)* Scope represents if this refers to a cluster or namespace scoped resource.
+      * **scope** ``str`` - *(optional)* scope represents if this refers to a cluster or namespace scoped resource.
         This may be set to "Cluster" (default) or "Namespace".
     """
     kind: 'str'
     name: 'str'
     apiGroup: 'str' = None
     namespace: 'str' = None
     scope: 'str' = None
@@ -199,35 +199,35 @@
 
 @dataclass
 class IngressClassSpec(DataclassDictMixIn):
     """IngressClassSpec provides information about the class of an Ingress.
 
       **parameters**
 
-      * **controller** ``str`` - *(optional)* Controller refers to the name of the controller that should handle this class.
+      * **controller** ``str`` - *(optional)* controller refers to the name of the controller that should handle this class.
         This allows for different "flavors" that are controlled by the same
-        controller. For example, you may have different Parameters for the same
+        controller. For example, you may have different parameters for the same
         implementing controller. This should be specified as a domain-prefixed path no
         more than 250 characters in length, e.g. "acme.io/ingress-controller". This
         field is immutable.
-      * **parameters** ``IngressClassParametersReference`` - *(optional)* Parameters is a link to a custom resource containing additional configuration
+      * **parameters** ``IngressClassParametersReference`` - *(optional)* parameters is a link to a custom resource containing additional configuration
         for the controller. This is optional if the controller does not require extra
         parameters.
     """
     controller: 'str' = None
     parameters: 'IngressClassParametersReference' = None
 
 
 @dataclass
 class IngressList(DataclassDictMixIn):
     """IngressList is a collection of Ingress.
 
       **parameters**
 
-      * **items** ``List[Ingress]`` - Items is the list of Ingress.
+      * **items** ``List[Ingress]`` - items is the list of Ingress.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
@@ -244,44 +244,44 @@
 @dataclass
 class IngressLoadBalancerIngress(DataclassDictMixIn):
     """IngressLoadBalancerIngress represents the status of a load-balancer ingress
       point.
 
       **parameters**
 
-      * **hostname** ``str`` - *(optional)* Hostname is set for load-balancer ingress points that are DNS based.
-      * **ip** ``str`` - *(optional)* IP is set for load-balancer ingress points that are IP based.
-      * **ports** ``List[IngressPortStatus]`` - *(optional)* Ports provides information about the ports exposed by this LoadBalancer.
+      * **hostname** ``str`` - *(optional)* hostname is set for load-balancer ingress points that are DNS based.
+      * **ip** ``str`` - *(optional)* ip is set for load-balancer ingress points that are IP based.
+      * **ports** ``List[IngressPortStatus]`` - *(optional)* ports provides information about the ports exposed by this LoadBalancer.
     """
     hostname: 'str' = None
     ip: 'str' = None
     ports: 'List[IngressPortStatus]' = None
 
 
 @dataclass
 class IngressLoadBalancerStatus(DataclassDictMixIn):
     """IngressLoadBalancerStatus represents the status of a load-balancer.
 
       **parameters**
 
-      * **ingress** ``List[IngressLoadBalancerIngress]`` - *(optional)* Ingress is a list containing ingress points for the load-balancer.
+      * **ingress** ``List[IngressLoadBalancerIngress]`` - *(optional)* ingress is a list containing ingress points for the load-balancer.
     """
     ingress: 'List[IngressLoadBalancerIngress]' = None
 
 
 @dataclass
 class IngressPortStatus(DataclassDictMixIn):
     """IngressPortStatus represents the error condition of a service port
 
       **parameters**
 
-      * **port** ``int`` - Port is the port number of the ingress port.
-      * **protocol** ``str`` - Protocol is the protocol of the ingress port. The supported values are: "TCP",
+      * **port** ``int`` - port is the port number of the ingress port.
+      * **protocol** ``str`` - protocol is the protocol of the ingress port. The supported values are: "TCP",
         "UDP", "SCTP"
-      * **error** ``str`` - *(optional)* Error is to record the problem with the service port The format of the error
+      * **error** ``str`` - *(optional)* error is to record the problem with the service port The format of the error
         shall comply with the following rules: - built-in error values shall be
         specified in this file and those shall use
           CamelCase names
         - cloud provider specific error values must have names that comply with the
           format foo.example.com/CamelCase.
     """
     port: 'int'
@@ -294,115 +294,115 @@
     """IngressRule represents the rules mapping the paths under a specified host to
       the related backend services. Incoming requests are first evaluated for a host
       match, then routed to the backend associated with the matching
       IngressRuleValue.
 
       **parameters**
 
-      * **host** ``str`` - *(optional)* Host is the fully qualified domain name of a network host, as defined by RFC
+      * **host** ``str`` - *(optional)* host is the fully qualified domain name of a network host, as defined by RFC
         3986. Note the following deviations from the "host" part of the URI as defined
         in RFC 3986: 1. IPs are not allowed. Currently an IngressRuleValue can only
         apply to
            the IP in the Spec of the parent Ingress.
         2. The `:` delimiter is not respected because ports are not allowed.
         	  Currently the port of an Ingress is implicitly :80 for http and
         	  :443 for https.
         Both these may change in the future. Incoming requests are matched against the
         host before the IngressRuleValue. If the host is unspecified, the Ingress
         routes all traffic based on the specified IngressRuleValue.
-        Host can be "precise" which is a domain name without the terminating dot of a
+        host can be "precise" which is a domain name without the terminating dot of a
         network host (e.g. "foo.bar.com") or "wildcard", which is a domain name
         prefixed with a single wildcard label (e.g. "*.foo.com"). The wildcard
         character '*' must appear by itself as the first DNS label and matches only a
         single label. You cannot have a wildcard label by itself (e.g. Host == "*").
         Requests will be matched against the Host field in the following way: 1. If
-        Host is precise, the request matches this rule if the http host header is
-        equal to Host. 2. If Host is a wildcard, then the request matches this rule if
+        host is precise, the request matches this rule if the http host header is
+        equal to Host. 2. If host is a wildcard, then the request matches this rule if
         the http host header is to equal to the suffix (removing the first label) of
         the wildcard rule.
       * **http** ``HTTPIngressRuleValue`` - *(optional)* 
     """
     host: 'str' = None
     http: 'HTTPIngressRuleValue' = None
 
 
 @dataclass
 class IngressServiceBackend(DataclassDictMixIn):
     """IngressServiceBackend references a Kubernetes Service as a Backend.
 
       **parameters**
 
-      * **name** ``str`` - Name is the referenced service. The service must exist in the same namespace
+      * **name** ``str`` - name is the referenced service. The service must exist in the same namespace
         as the Ingress object.
-      * **port** ``ServiceBackendPort`` - *(optional)* Port of the referenced service. A port name or port number is required for a
+      * **port** ``ServiceBackendPort`` - *(optional)* port of the referenced service. A port name or port number is required for a
         IngressServiceBackend.
     """
     name: 'str'
     port: 'ServiceBackendPort' = None
 
 
 @dataclass
 class IngressSpec(DataclassDictMixIn):
     """IngressSpec describes the Ingress the user wishes to exist.
 
       **parameters**
 
-      * **defaultBackend** ``IngressBackend`` - *(optional)* DefaultBackend is the backend that should handle requests that don't match any
+      * **defaultBackend** ``IngressBackend`` - *(optional)* defaultBackend is the backend that should handle requests that don't match any
         rule. If Rules are not specified, DefaultBackend must be specified. If
         DefaultBackend is not set, the handling of requests that do not match any of
         the rules will be up to the Ingress controller.
-      * **ingressClassName** ``str`` - *(optional)* IngressClassName is the name of an IngressClass cluster resource. Ingress
+      * **ingressClassName** ``str`` - *(optional)* ingressClassName is the name of an IngressClass cluster resource. Ingress
         controller implementations use this field to know whether they should be
         serving this Ingress resource, by a transitive connection (controller ->
         IngressClass -> Ingress resource). Although the `kubernetes.io/ingress.class`
         annotation (simple constant name) was never formally defined, it was widely
         supported by Ingress controllers to create a direct binding between Ingress
         controller and Ingress resources. Newly created Ingress resources should
         prefer using the field. However, even though the annotation is officially
         deprecated, for backwards compatibility reasons, ingress controllers should
         still honor that annotation if present.
-      * **rules** ``List[IngressRule]`` - *(optional)* A list of host rules used to configure the Ingress. If unspecified, or no rule
-        matches, all traffic is sent to the default backend.
-      * **tls** ``List[IngressTLS]`` - *(optional)* TLS configuration. Currently the Ingress only supports a single TLS port, 443.
-        If multiple members of this list specify different hosts, they will be
-        multiplexed on the same port according to the hostname specified through the
-        SNI TLS extension, if the ingress controller fulfilling the ingress supports
-        SNI.
+      * **rules** ``List[IngressRule]`` - *(optional)* rules is a list of host rules used to configure the Ingress. If unspecified,
+        or no rule matches, all traffic is sent to the default backend.
+      * **tls** ``List[IngressTLS]`` - *(optional)* tls represents the TLS configuration. Currently the Ingress only supports a
+        single TLS port, 443. If multiple members of this list specify different
+        hosts, they will be multiplexed on the same port according to the hostname
+        specified through the SNI TLS extension, if the ingress controller fulfilling
+        the ingress supports SNI.
     """
     defaultBackend: 'IngressBackend' = None
     ingressClassName: 'str' = None
     rules: 'List[IngressRule]' = None
     tls: 'List[IngressTLS]' = None
 
 
 @dataclass
 class IngressStatus(DataclassDictMixIn):
     """IngressStatus describe the current state of the Ingress.
 
       **parameters**
 
-      * **loadBalancer** ``IngressLoadBalancerStatus`` - *(optional)* LoadBalancer contains the current status of the load-balancer.
+      * **loadBalancer** ``IngressLoadBalancerStatus`` - *(optional)* loadBalancer contains the current status of the load-balancer.
     """
     loadBalancer: 'IngressLoadBalancerStatus' = None
 
 
 @dataclass
 class IngressTLS(DataclassDictMixIn):
-    """IngressTLS describes the transport layer security associated with an Ingress.
+    """IngressTLS describes the transport layer security associated with an ingress.
 
       **parameters**
 
-      * **hosts** ``List[str]`` - *(optional)* Hosts are a list of hosts included in the TLS certificate. The values in this
+      * **hosts** ``List[str]`` - *(optional)* hosts is a list of hosts included in the TLS certificate. The values in this
         list must match the name/s used in the tlsSecret. Defaults to the wildcard
         host setting for the loadbalancer controller fulfilling this Ingress, if left
         unspecified.
-      * **secretName** ``str`` - *(optional)* SecretName is the name of the secret used to terminate TLS traffic on port
+      * **secretName** ``str`` - *(optional)* secretName is the name of the secret used to terminate TLS traffic on port
         443. Field is left optional to allow TLS routing based on SNI hostname alone.
         If the SNI host in a listener conflicts with the "Host" header field used by
-        an IngressRule, the SNI host is used for termination and value of the Host
+        an IngressRule, the SNI host is used for termination and value of the "Host"
         header is used for routing.
     """
     hosts: 'List[str]' = None
     secretName: 'str' = None
 
 
 @dataclass
@@ -417,16 +417,17 @@
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object's metadata. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **spec** ``NetworkPolicySpec`` - *(optional)* Specification of the desired behavior for this NetworkPolicy.
-      * **status** ``NetworkPolicyStatus`` - *(optional)* Status is the current state of the NetworkPolicy. More info:
+      * **spec** ``NetworkPolicySpec`` - *(optional)* spec represents the specification of the desired behavior for this
+        NetworkPolicy.
+      * **status** ``NetworkPolicyStatus`` - *(optional)* status represents the current state of the NetworkPolicy. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status
     """
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
     spec: 'NetworkPolicySpec' = None
     status: 'NetworkPolicyStatus' = None
@@ -436,61 +437,61 @@
 class NetworkPolicyEgressRule(DataclassDictMixIn):
     """NetworkPolicyEgressRule describes a particular set of traffic that is allowed
       out of pods matched by a NetworkPolicySpec's podSelector. The traffic must
       match both ports and to. This type is beta-level in 1.8
 
       **parameters**
 
-      * **ports** ``List[NetworkPolicyPort]`` - *(optional)* List of destination ports for outgoing traffic. Each item in this list is
-        combined using a logical OR. If this field is empty or missing, this rule
-        matches all ports (traffic not restricted by port). If this field is present
-        and contains at least one item, then this rule allows traffic only if the
-        traffic matches at least one port in the list.
-      * **to** ``List[NetworkPolicyPeer]`` - *(optional)* List of destinations for outgoing traffic of pods selected for this rule.
-        Items in this list are combined using a logical OR operation. If this field is
-        empty or missing, this rule matches all destinations (traffic not restricted
-        by destination). If this field is present and contains at least one item, this
-        rule allows traffic only if the traffic matches at least one item in the to
-        list.
+      * **ports** ``List[NetworkPolicyPort]`` - *(optional)* ports is a list of destination ports for outgoing traffic. Each item in this
+        list is combined using a logical OR. If this field is empty or missing, this
+        rule matches all ports (traffic not restricted by port). If this field is
+        present and contains at least one item, then this rule allows traffic only if
+        the traffic matches at least one port in the list.
+      * **to** ``List[NetworkPolicyPeer]`` - *(optional)* to is a list of destinations for outgoing traffic of pods selected for this
+        rule. Items in this list are combined using a logical OR operation. If this
+        field is empty or missing, this rule matches all destinations (traffic not
+        restricted by destination). If this field is present and contains at least one
+        item, this rule allows traffic only if the traffic matches at least one item
+        in the to list.
     """
     ports: 'List[NetworkPolicyPort]' = None
     to: 'List[NetworkPolicyPeer]' = None
 
 
 @dataclass
 class NetworkPolicyIngressRule(DataclassDictMixIn):
     """NetworkPolicyIngressRule describes a particular set of traffic that is allowed
       to the pods matched by a NetworkPolicySpec's podSelector. The traffic must
       match both ports and from.
 
       **parameters**
 
-      * **from_** ``List[NetworkPolicyPeer]`` - *(optional)* List of sources which should be able to access the pods selected for this
-        rule. Items in this list are combined using a logical OR operation. If this
-        field is empty or missing, this rule matches all sources (traffic not
+      * **from_** ``List[NetworkPolicyPeer]`` - *(optional)* from is a list of sources which should be able to access the pods selected for
+        this rule. Items in this list are combined using a logical OR operation. If
+        this field is empty or missing, this rule matches all sources (traffic not
         restricted by source). If this field is present and contains at least one
         item, this rule allows traffic only if the traffic matches at least one item
         in the from list.
-      * **ports** ``List[NetworkPolicyPort]`` - *(optional)* List of ports which should be made accessible on the pods selected for this
-        rule. Each item in this list is combined using a logical OR. If this field is
-        empty or missing, this rule matches all ports (traffic not restricted by
-        port). If this field is present and contains at least one item, then this rule
-        allows traffic only if the traffic matches at least one port in the list.
+      * **ports** ``List[NetworkPolicyPort]`` - *(optional)* ports is a list of ports which should be made accessible on the pods selected
+        for this rule. Each item in this list is combined using a logical OR. If this
+        field is empty or missing, this rule matches all ports (traffic not restricted
+        by port). If this field is present and contains at least one item, then this
+        rule allows traffic only if the traffic matches at least one port in the list.
     """
     from_: 'List[NetworkPolicyPeer]' = field(metadata={"json": "from"}, default=None)
     ports: 'List[NetworkPolicyPort]' = None
 
 
 @dataclass
 class NetworkPolicyList(DataclassDictMixIn):
     """NetworkPolicyList is a list of NetworkPolicy objects.
 
       **parameters**
 
-      * **items** ``List[NetworkPolicy]`` - Items is a list of schema objects.
+      * **items** ``List[NetworkPolicy]`` - items is a list of schema objects.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
@@ -507,119 +508,120 @@
 @dataclass
 class NetworkPolicyPeer(DataclassDictMixIn):
     """NetworkPolicyPeer describes a peer to allow traffic to/from. Only certain
       combinations of fields are allowed
 
       **parameters**
 
-      * **ipBlock** ``IPBlock`` - *(optional)* IPBlock defines policy on a particular IPBlock. If this field is set then
+      * **ipBlock** ``IPBlock`` - *(optional)* ipBlock defines policy on a particular IPBlock. If this field is set then
         neither of the other fields can be.
-      * **namespaceSelector** ``meta_v1.LabelSelector`` - *(optional)* Selects Namespaces using cluster-scoped labels. This field follows standard
-        label selector semantics; if present but empty, it selects all namespaces.
-        If PodSelector is also set, then the NetworkPolicyPeer as a whole selects the
-        Pods matching PodSelector in the Namespaces selected by NamespaceSelector.
-        Otherwise it selects all Pods in the Namespaces selected by NamespaceSelector.
-      * **podSelector** ``meta_v1.LabelSelector`` - *(optional)* This is a label selector which selects Pods. This field follows standard label
-        selector semantics; if present but empty, it selects all pods.
-        If NamespaceSelector is also set, then the NetworkPolicyPeer as a whole
-        selects the Pods matching PodSelector in the Namespaces selected by
-        NamespaceSelector. Otherwise it selects the Pods matching PodSelector in the
-        policy's own Namespace.
+      * **namespaceSelector** ``meta_v1.LabelSelector`` - *(optional)* namespaceSelector selects namespaces using cluster-scoped labels. This field
+        follows standard label selector semantics; if present but empty, it selects
+        all namespaces.
+        If podSelector is also set, then the NetworkPolicyPeer as a whole selects the
+        pods matching podSelector in the namespaces selected by namespaceSelector.
+        Otherwise it selects all pods in the namespaces selected by namespaceSelector.
+      * **podSelector** ``meta_v1.LabelSelector`` - *(optional)* podSelector is a label selector which selects pods. This field follows
+        standard label selector semantics; if present but empty, it selects all pods.
+        If namespaceSelector is also set, then the NetworkPolicyPeer as a whole
+        selects the pods matching podSelector in the Namespaces selected by
+        NamespaceSelector. Otherwise it selects the pods matching podSelector in the
+        policy's own namespace.
     """
     ipBlock: 'IPBlock' = None
     namespaceSelector: 'meta_v1.LabelSelector' = None
     podSelector: 'meta_v1.LabelSelector' = None
 
 
 @dataclass
 class NetworkPolicyPort(DataclassDictMixIn):
     """NetworkPolicyPort describes a port to allow traffic on
 
       **parameters**
 
-      * **endPort** ``int`` - *(optional)* If set, indicates that the range of ports from port to endPort, inclusive,
-        should be allowed by the policy. This field cannot be defined if the port
-        field is not defined or if the port field is defined as a named (string) port.
-        The endPort must be equal or greater than port.
-      * **port** ``util_intstr.IntOrString`` - *(optional)* The port on the given protocol. This can either be a numerical or named port
-        on a pod. If this field is not provided, this matches all port names and
-        numbers. If present, only traffic on the specified protocol AND port will be
-        matched.
-      * **protocol** ``str`` - *(optional)* The protocol (TCP, UDP, or SCTP) which traffic must match. If not specified,
-        this field defaults to TCP.
+      * **endPort** ``int`` - *(optional)* endPort indicates that the range of ports from port to endPort if set,
+        inclusive, should be allowed by the policy. This field cannot be defined if
+        the port field is not defined or if the port field is defined as a named
+        (string) port. The endPort must be equal or greater than port.
+      * **port** ``util_intstr.IntOrString`` - *(optional)* port represents the port on the given protocol. This can either be a numerical
+        or named port on a pod. If this field is not provided, this matches all port
+        names and numbers. If present, only traffic on the specified protocol AND port
+        will be matched.
+      * **protocol** ``str`` - *(optional)* protocol represents the protocol (TCP, UDP, or SCTP) which traffic must match.
+        If not specified, this field defaults to TCP.
     """
     endPort: 'int' = None
     port: 'util_intstr.IntOrString' = None
     protocol: 'str' = None
 
 
 @dataclass
 class NetworkPolicySpec(DataclassDictMixIn):
     """NetworkPolicySpec provides the specification of a NetworkPolicy
 
       **parameters**
 
-      * **podSelector** ``meta_v1.LabelSelector`` - Selects the pods to which this NetworkPolicy object applies. The array of
-        ingress rules is applied to any pods selected by this field. Multiple network
-        policies can select the same set of pods. In this case, the ingress rules for
-        each are combined additively. This field is NOT optional and follows standard
-        label selector semantics. An empty podSelector matches all pods in this
-        namespace.
-      * **egress** ``List[NetworkPolicyEgressRule]`` - *(optional)* List of egress rules to be applied to the selected pods. Outgoing traffic is
-        allowed if there are no NetworkPolicies selecting the pod (and cluster policy
-        otherwise allows the traffic), OR if the traffic matches at least one egress
-        rule across all of the NetworkPolicy objects whose podSelector matches the
-        pod. If this field is empty then this NetworkPolicy limits all outgoing
-        traffic (and serves solely to ensure that the pods it selects are isolated by
-        default). This field is beta-level in 1.8
-      * **ingress** ``List[NetworkPolicyIngressRule]`` - *(optional)* List of ingress rules to be applied to the selected pods. Traffic is allowed
-        to a pod if there are no NetworkPolicies selecting the pod (and cluster policy
-        otherwise allows the traffic), OR if the traffic source is the pod's local
-        node, OR if the traffic matches at least one ingress rule across all of the
-        NetworkPolicy objects whose podSelector matches the pod. If this field is
-        empty then this NetworkPolicy does not allow any traffic (and serves solely to
-        ensure that the pods it selects are isolated by default)
-      * **policyTypes** ``List[str]`` - *(optional)* List of rule types that the NetworkPolicy relates to. Valid options are
-        ["Ingress"], ["Egress"], or ["Ingress", "Egress"]. If this field is not
-        specified, it will default based on the existence of Ingress or Egress rules;
-        policies that contain an Egress section are assumed to affect Egress, and all
-        policies (whether or not they contain an Ingress section) are assumed to
-        affect Ingress. If you want to write an egress-only policy, you must
+      * **podSelector** ``meta_v1.LabelSelector`` - podSelector selects the pods to which this NetworkPolicy object applies. The
+        array of ingress rules is applied to any pods selected by this field. Multiple
+        network policies can select the same set of pods. In this case, the ingress
+        rules for each are combined additively. This field is NOT optional and follows
+        standard label selector semantics. An empty podSelector matches all pods in
+        this namespace.
+      * **egress** ``List[NetworkPolicyEgressRule]`` - *(optional)* egress is a list of egress rules to be applied to the selected pods. Outgoing
+        traffic is allowed if there are no NetworkPolicies selecting the pod (and
+        cluster policy otherwise allows the traffic), OR if the traffic matches at
+        least one egress rule across all of the NetworkPolicy objects whose
+        podSelector matches the pod. If this field is empty then this NetworkPolicy
+        limits all outgoing traffic (and serves solely to ensure that the pods it
+        selects are isolated by default). This field is beta-level in 1.8
+      * **ingress** ``List[NetworkPolicyIngressRule]`` - *(optional)* ingress is a list of ingress rules to be applied to the selected pods. Traffic
+        is allowed to a pod if there are no NetworkPolicies selecting the pod (and
+        cluster policy otherwise allows the traffic), OR if the traffic source is the
+        pod's local node, OR if the traffic matches at least one ingress rule across
+        all of the NetworkPolicy objects whose podSelector matches the pod. If this
+        field is empty then this NetworkPolicy does not allow any traffic (and serves
+        solely to ensure that the pods it selects are isolated by default)
+      * **policyTypes** ``List[str]`` - *(optional)* policyTypes is a list of rule types that the NetworkPolicy relates to. Valid
+        options are ["Ingress"], ["Egress"], or ["Ingress", "Egress"]. If this field
+        is not specified, it will default based on the existence of ingress or egress
+        rules; policies that contain an egress section are assumed to affect egress,
+        and all policies (whether or not they contain an ingress section) are assumed
+        to affect ingress. If you want to write an egress-only policy, you must
         explicitly specify policyTypes [ "Egress" ]. Likewise, if you want to write a
         policy that specifies that no egress is allowed, you must specify a
         policyTypes value that include "Egress" (since such a policy would not include
-        an Egress section and would otherwise default to just [ "Ingress" ]). This
+        an egress section and would otherwise default to just [ "Ingress" ]). This
         field is beta-level in 1.8
     """
     podSelector: 'meta_v1.LabelSelector'
     egress: 'List[NetworkPolicyEgressRule]' = None
     ingress: 'List[NetworkPolicyIngressRule]' = None
     policyTypes: 'List[str]' = None
 
 
 @dataclass
 class NetworkPolicyStatus(DataclassDictMixIn):
-    """NetworkPolicyStatus describe the current state of the NetworkPolicy.
+    """NetworkPolicyStatus describes the current state of the NetworkPolicy.
 
       **parameters**
 
-      * **conditions** ``List[meta_v1.Condition]`` - *(optional)* Conditions holds an array of metav1.Condition that describe the state of the
+      * **conditions** ``List[meta_v1.Condition]`` - *(optional)* conditions holds an array of metav1.Condition that describe the state of the
         NetworkPolicy. Current service state
     """
     conditions: 'List[meta_v1.Condition]' = None
 
 
 @dataclass
 class ServiceBackendPort(DataclassDictMixIn):
     """ServiceBackendPort is the service port being referenced.
 
       **parameters**
 
-      * **name** ``str`` - *(optional)* Name is the name of the port on the Service. This is a mutually exclusive
+      * **name** ``str`` - *(optional)* name is the name of the port on the Service. This is a mutually exclusive
         setting with "Number".
-      * **number** ``int`` - *(optional)* Number is the numerical port number (e.g. 80) on the Service. This is a
+      * **number** ``int`` - *(optional)* number is the numerical port number (e.g. 80) on the Service. This is a
         mutually exclusive setting with "Name".
     """
     name: 'str' = None
     number: 'int' = None
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/node_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/node_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from . import core_v1
 from . import meta_v1
+from . import core_v1
 
 
 @dataclass
 class Overhead(DataclassDictMixIn):
     """Overhead structure represents the resource overhead associated with running a
       pod.
 
       **parameters**
 
-      * **podFixed** ``dict`` - *(optional)* PodFixed represents the fixed resource overhead associated with running a pod.
+      * **podFixed** ``dict`` - *(optional)* podFixed represents the fixed resource overhead associated with running a pod.
     """
     podFixed: 'dict' = None
 
 
 @dataclass
 class RuntimeClass(DataclassDictMixIn):
     """RuntimeClass defines a class of container runtime supported in the cluster.
@@ -27,15 +27,15 @@
       all containers in a pod. RuntimeClasses are manually defined by a user or
       cluster provisioner, and referenced in the PodSpec. The Kubelet is responsible
       for resolving the RuntimeClassName reference before running the pod.  For more
       details, see https://kubernetes.io/docs/concepts/containers/runtime-class/
 
       **parameters**
 
-      * **handler** ``str`` - Handler specifies the underlying runtime and configuration that the CRI
+      * **handler** ``str`` - handler specifies the underlying runtime and configuration that the CRI
         implementation will use to handle pods of this class. The possible values are
         specific to the node & CRI configuration.  It is assumed that all handlers are
         available on every node, and handlers of the same name are equivalent on every
         node. For example, a handler called "runc" might specify that the runc OCI
         runtime (using native Linux containers) will be used to run the containers in
         a pod. The Handler must be lowercase, conform to the DNS Label (RFC 1123)
         requirements, and is immutable.
@@ -45,18 +45,18 @@
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **overhead** ``Overhead`` - *(optional)* Overhead represents the resource overhead associated with running a pod for a
+      * **overhead** ``Overhead`` - *(optional)* overhead represents the resource overhead associated with running a pod for a
         given RuntimeClass. For more details, see
          https://kubernetes.io/docs/concepts/scheduling-eviction/pod-overhead/
-      * **scheduling** ``Scheduling`` - *(optional)* Scheduling holds the scheduling constraints to ensure that pods running with
+      * **scheduling** ``Scheduling`` - *(optional)* scheduling holds the scheduling constraints to ensure that pods running with
         this RuntimeClass are scheduled to nodes that support it. If scheduling is
         nil, this RuntimeClass is assumed to be supported by all nodes.
     """
     handler: 'str'
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
@@ -66,15 +66,15 @@
 
 @dataclass
 class RuntimeClassList(DataclassDictMixIn):
     """RuntimeClassList is a list of RuntimeClass objects.
 
       **parameters**
 
-      * **items** ``List[RuntimeClass]`` - Items is a list of schema objects.
+      * **items** ``List[RuntimeClass]`` - items is a list of schema objects.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/policy_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/policy_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from . import util_intstr
 from . import meta_v1
+from . import util_intstr
 
 
 @dataclass
 class Eviction(DataclassDictMixIn):
     """Eviction evicts a pod from its node subject to certain policies and safety
       constraints. This is a subresource of Pod.  A request to cause such an
       eviction is created by POSTing to .../pods/<pod name>/evictions.
@@ -115,16 +115,16 @@
         not yet healthy are considered disrupted and can be evicted regardless of
         whether the criteria in a PDB is met. This means perspective running pods of a
         disrupted application might not get a chance to become healthy. Healthy pods
         will be subject to the PDB for eviction.
         Additional policies may be added in the future. Clients making eviction
         decisions should disallow eviction of unhealthy pods if they encounter an
         unrecognized policy in this field.
-        This field is alpha-level. The eviction API uses this field when the feature
-        gate PDBUnhealthyPodEvictionPolicy is enabled (disabled by default).
+        This field is beta-level. The eviction API uses this field when the feature
+        gate PDBUnhealthyPodEvictionPolicy is enabled (enabled by default).
     """
     maxUnavailable: 'util_intstr.IntOrString' = None
     minAvailable: 'util_intstr.IntOrString' = None
     selector: 'meta_v1.LabelSelector' = None
     unhealthyPodEvictionPolicy: 'str' = None
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/rbac_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/rbac_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/models/resource_v1alpha1.py` & `lightkube-models-1.27.1.4/lightkube/models/resource_v1alpha2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,101 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from . import meta_v1
 from . import core_v1
+from . import meta_v1
 
 
 @dataclass
 class AllocationResult(DataclassDictMixIn):
-    """AllocationResult contains attributed of an allocated resource.
+    """AllocationResult contains attributes of an allocated resource.
 
       **parameters**
 
       * **availableOnNodes** ``core_v1.NodeSelector`` - *(optional)* This field will get set by the resource driver after it has allocated the
-        resource driver to inform the scheduler where it can schedule Pods using the
+        resource to inform the scheduler where it can schedule Pods using the
         ResourceClaim.
         Setting this field is optional. If null, the resource is available everywhere.
-      * **resourceHandle** ``str`` - *(optional)* ResourceHandle contains arbitrary data returned by the driver after a
-        successful allocation. This is opaque for Kubernetes. Driver documentation may
-        explain to users how to interpret this data if needed.
-        The maximum size of this field is 16KiB. This may get increased in the future,
-        but not reduced.
+      * **resourceHandles** ``List[ResourceHandle]`` - *(optional)* ResourceHandles contain the state associated with an allocation that should be
+        maintained throughout the lifetime of a claim. Each ResourceHandle contains
+        data that should be passed to a specific kubelet plugin once it lands on a
+        node. This data is returned by the driver after a successful allocation and is
+        opaque to Kubernetes. Driver documentation may explain to users how to
+        interpret this data if needed.
+        Setting this field is optional. It has a maximum size of 32 entries. If null
+        (or empty), it is assumed this allocation will be processed by a single
+        kubelet plugin with no ResourceHandle data attached. The name of the kubelet
+        plugin invoked will match the DriverName set in the ResourceClaimStatus this
+        AllocationResult is embedded in.
       * **shareable** ``bool`` - *(optional)* Shareable determines whether the resource supports more than one consumer at a
         time.
     """
     availableOnNodes: 'core_v1.NodeSelector' = None
-    resourceHandle: 'str' = None
+    resourceHandles: 'List[ResourceHandle]' = None
     shareable: 'bool' = None
 
 
 @dataclass
-class PodScheduling(DataclassDictMixIn):
-    """PodScheduling objects hold information that is needed to schedule a Pod with
-      ResourceClaims that use "WaitForFirstConsumer" allocation mode.
+class PodSchedulingContext(DataclassDictMixIn):
+    """PodSchedulingContext objects hold information that is needed to schedule a Pod
+      with ResourceClaims that use "WaitForFirstConsumer" allocation mode.
       
       This is an alpha type and requires enabling the DynamicResourceAllocation
       feature gate.
 
       **parameters**
 
-      * **spec** ``PodSchedulingSpec`` - Spec describes where resources for the Pod are needed.
+      * **spec** ``PodSchedulingContextSpec`` - Spec describes where resources for the Pod are needed.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object metadata
-      * **status** ``PodSchedulingStatus`` - *(optional)* Status describes where resources for the Pod can be allocated.
+      * **status** ``PodSchedulingContextStatus`` - *(optional)* Status describes where resources for the Pod can be allocated.
     """
-    spec: 'PodSchedulingSpec'
+    spec: 'PodSchedulingContextSpec'
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
-    status: 'PodSchedulingStatus' = None
+    status: 'PodSchedulingContextStatus' = None
 
 
 @dataclass
-class PodSchedulingList(DataclassDictMixIn):
-    """PodSchedulingList is a collection of Pod scheduling objects.
+class PodSchedulingContextList(DataclassDictMixIn):
+    """PodSchedulingContextList is a collection of Pod scheduling objects.
 
       **parameters**
 
-      * **items** ``List[PodScheduling]`` - Items is the list of PodScheduling objects.
+      * **items** ``List[PodSchedulingContext]`` - Items is the list of PodSchedulingContext objects.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ListMeta`` - *(optional)* Standard list metadata
     """
-    items: 'List[PodScheduling]'
+    items: 'List[PodSchedulingContext]'
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ListMeta' = None
 
 
 @dataclass
-class PodSchedulingSpec(DataclassDictMixIn):
-    """PodSchedulingSpec describes where resources for the Pod are needed.
+class PodSchedulingContextSpec(DataclassDictMixIn):
+    """PodSchedulingContextSpec describes where resources for the Pod are needed.
 
       **parameters**
 
       * **potentialNodes** ``List[str]`` - *(optional)* PotentialNodes lists nodes where the Pod might be able to run.
         The size of this field is limited to 128. This is large enough for many
         clusters. Larger clusters may need more attempts to find a node that suits all
         pending resources. This may get increased in the future, but not reduced.
@@ -98,16 +104,17 @@
         attempted.
     """
     potentialNodes: 'List[str]' = None
     selectedNode: 'str' = None
 
 
 @dataclass
-class PodSchedulingStatus(DataclassDictMixIn):
-    """PodSchedulingStatus describes where resources for the Pod can be allocated.
+class PodSchedulingContextStatus(DataclassDictMixIn):
+    """PodSchedulingContextStatus describes where resources for the Pod can be
+      allocated.
 
       **parameters**
 
       * **resourceClaims** ``List[ResourceClaimSchedulingStatus]`` - *(optional)* ResourceClaims describes resource availability for each pod.spec.resourceClaim
         entry where the corresponding ResourceClaim uses "WaitForFirstConsumer"
         allocation mode.
     """
@@ -248,16 +255,17 @@
 @dataclass
 class ResourceClaimStatus(DataclassDictMixIn):
     """ResourceClaimStatus tracks whether the resource has been allocated and what
       the resulting attributes are.
 
       **parameters**
 
-      * **allocation** ``AllocationResult`` - *(optional)* Allocation is set by the resource driver once a resource has been allocated
-        successfully. If this is not specified, the resource is not yet allocated.
+      * **allocation** ``AllocationResult`` - *(optional)* Allocation is set by the resource driver once a resource or set of resources
+        has been allocated successfully. If this is not specified, the resources have
+        not been allocated yet.
       * **deallocationRequested** ``bool`` - *(optional)* DeallocationRequested indicates that a ResourceClaim is to be deallocated.
         The driver then must deallocate this claim and reset the field together with
         clearing the Allocation field.
         While DeallocationRequested is set, no new consumers may be added to
         ReservedFor.
       * **driverName** ``str`` - *(optional)* DriverName is a copy of the driver name from the ResourceClass at the time
         when allocation started.
@@ -420,7 +428,30 @@
     """
     kind: 'str'
     name: 'str'
     apiGroup: 'str' = None
     namespace: 'str' = None
 
 
+@dataclass
+class ResourceHandle(DataclassDictMixIn):
+    """ResourceHandle holds opaque resource data for processing by a specific kubelet
+      plugin.
+
+      **parameters**
+
+      * **data** ``str`` - *(optional)* Data contains the opaque data associated with this ResourceHandle. It is set
+        by the controller component of the resource driver whose name matches the
+        DriverName set in the ResourceClaimStatus this ResourceHandle is embedded in.
+        It is set at allocation time and is intended for processing by the kubelet
+        plugin whose name matches the DriverName set in this ResourceHandle.
+        The maximum size of this field is 16KiB. This may get increased in the future,
+        but not reduced.
+      * **driverName** ``str`` - *(optional)* DriverName specifies the name of the resource driver whose kubelet plugin
+        should be invoked to process this ResourceHandle's data once it lands on a
+        node. This may differ from the DriverName set in ResourceClaimStatus this
+        ResourceHandle is embedded in.
+    """
+    data: 'str' = None
+    driverName: 'str' = None
+
+
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/scheduling_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/scheduling_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 @dataclass
 class PriorityClass(DataclassDictMixIn):
     """PriorityClass defines mapping from a priority class name to the priority
       integer value. The value can be any valid integer.
 
       **parameters**
 
-      * **value** ``int`` - The value of this priority class. This is the actual priority that pods
-        receive when they have the name of this class in their pod spec.
+      * **value** ``int`` - value represents the integer value of this priority class. This is the actual
+        priority that pods receive when they have the name of this class in their pod
+        spec.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **description** ``str`` - *(optional)* description is an arbitrary string that usually provides guidelines on when
         this priority class should be used.
       * **globalDefault** ``bool`` - *(optional)* globalDefault specifies whether this PriorityClass should be considered as the
@@ -30,15 +31,15 @@
         default priority.
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object's metadata. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **preemptionPolicy** ``str`` - *(optional)* PreemptionPolicy is the Policy for preempting pods with lower priority. One of
+      * **preemptionPolicy** ``str`` - *(optional)* preemptionPolicy is the Policy for preempting pods with lower priority. One of
         Never, PreemptLowerPriority. Defaults to PreemptLowerPriority if unset.
     """
     value: 'int'
     apiVersion: 'str' = None
     description: 'str' = None
     globalDefault: 'bool' = None
     kind: 'str' = None
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/storage_v1.py` & `lightkube-models-1.27.1.4/lightkube/models/storage_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # autogenerated module
 from dataclasses import dataclass, field
 from typing import List
 
 from ..core.dataclasses_dict import DataclassDictMixIn
 
-from . import core_v1
 from . import meta_v1
 from . import resource
+from . import core_v1
 
 
 @dataclass
 class CSIDriver(DataclassDictMixIn):
     """CSIDriver captures information about a Container Storage Interface (CSI)
       volume driver deployed on the cluster. Kubernetes attach detach controller
       uses this object to determine whether attach is required. Kubelet uses this
       object to determine whether pod information needs to be passed on mount.
       CSIDriver objects are non-namespaced.
 
       **parameters**
 
-      * **spec** ``CSIDriverSpec`` - Specification of the CSI Driver.
+      * **spec** ``CSIDriverSpec`` - spec represents the specification of the CSI Driver.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
@@ -77,73 +77,75 @@
         which checks the volumeattachment status and waits until the volume is
         attached before proceeding to mounting. The CSI external-attacher coordinates
         with CSI volume driver and updates the volumeattachment status when the attach
         operation is complete. If the CSIDriverRegistry feature gate is enabled and
         the value is specified to false, the attach operation will be skipped.
         Otherwise the attach operation will be called.
         This field is immutable.
-      * **fsGroupPolicy** ``str`` - *(optional)* Defines if the underlying volume supports changing ownership and permission of
-        the volume before being mounted. Refer to the specific FSGroupPolicy values
-        for additional details.
+      * **fsGroupPolicy** ``str`` - *(optional)* fsGroupPolicy defines if the underlying volume supports changing ownership and
+        permission of the volume before being mounted. Refer to the specific
+        FSGroupPolicy values for additional details.
         This field is immutable.
         Defaults to ReadWriteOnceWithFSType, which will examine each volume to
         determine if Kubernetes should modify ownership and permissions of the volume.
         With the default policy the defined fsGroup will only be applied if a fstype
         is defined and the volume's access mode contains ReadWriteOnce.
-      * **podInfoOnMount** ``bool`` - *(optional)* If set to true, podInfoOnMount indicates this CSI volume driver requires
-        additional pod information (like podName, podUID, etc.) during mount
-        operations. If set to false, pod information will not be passed on mount.
-        Default is false. The CSI driver specifies podInfoOnMount as part of driver
-        deployment. If true, Kubelet will pass pod information as VolumeContext in the
-        CSI NodePublishVolume() calls. The CSI driver is responsible for parsing and
-        validating the information passed in as VolumeContext. The following
-        VolumeConext will be passed if podInfoOnMount is set to true. This list might
-        grow, but the prefix will be used. "csi.storage.k8s.io/pod.name": pod.Name
-        "csi.storage.k8s.io/pod.namespace": pod.Namespace
-        "csi.storage.k8s.io/pod.uid": string(pod.UID) "csi.storage.k8s.io/ephemeral":
-        "true" if the volume is an ephemeral inline volume
+      * **podInfoOnMount** ``bool`` - *(optional)* podInfoOnMount indicates this CSI volume driver requires additional pod
+        information (like podName, podUID, etc.) during mount operations, if set to
+        true. If set to false, pod information will not be passed on mount. Default is
+        false.
+        The CSI driver specifies podInfoOnMount as part of driver deployment. If true,
+        Kubelet will pass pod information as VolumeContext in the CSI
+        NodePublishVolume() calls. The CSI driver is responsible for parsing and
+        validating the information passed in as VolumeContext.
+        The following VolumeConext will be passed if podInfoOnMount is set to true.
+        This list might grow, but the prefix will be used.
+        "csi.storage.k8s.io/pod.name": pod.Name "csi.storage.k8s.io/pod.namespace":
+        pod.Namespace "csi.storage.k8s.io/pod.uid": string(pod.UID)
+        "csi.storage.k8s.io/ephemeral": "true" if the volume is an ephemeral inline
+        volume
                                         defined by a CSIVolumeSource, otherwise
         "false"
         "csi.storage.k8s.io/ephemeral" is a new feature in Kubernetes 1.16. It is only
         required for drivers which support both the "Persistent" and "Ephemeral"
         VolumeLifecycleMode. Other drivers can leave pod info disabled and/or ignore
         this field. As Kubernetes 1.15 doesn't support this field, drivers can only
         support one mode when deployed on such a cluster and the deployment determines
         which mode that is, for example via a command line parameter of the driver.
         This field is immutable.
-      * **requiresRepublish** ``bool`` - *(optional)* RequiresRepublish indicates the CSI driver wants `NodePublishVolume` being
+      * **requiresRepublish** ``bool`` - *(optional)* requiresRepublish indicates the CSI driver wants `NodePublishVolume` being
         periodically called to reflect any possible change in the mounted volume. This
         field defaults to false.
         Note: After a successful initial NodePublishVolume call, subsequent calls to
         NodePublishVolume should only update the contents of the volume. New mount
         points will not be seen by a running container.
-      * **seLinuxMount** ``bool`` - *(optional)* SELinuxMount specifies if the CSI driver supports "-o context" mount option.
+      * **seLinuxMount** ``bool`` - *(optional)* seLinuxMount specifies if the CSI driver supports "-o context" mount option.
         When "true", the CSI driver must ensure that all volumes provided by this CSI
         driver can be mounted separately with different `-o context` options. This is
         typical for storage backends that provide volumes as filesystems on block
         devices or as independent shared volumes. Kubernetes will call NodeStage /
         NodePublish with "-o context=xyz" mount option when mounting a
         ReadWriteOncePod volume used in Pod that has explicitly set SELinux context.
         In the future, it may be expanded to other volume AccessModes. In any case,
         Kubernetes will ensure that the volume is mounted only with a single SELinux
         context.
         When "false", Kubernetes won't pass any special SELinux mount options to the
         driver. This is typical for volumes that represent subdirectories of a bigger
         shared filesystem.
         Default is "false".
-      * **storageCapacity** ``bool`` - *(optional)* If set to true, storageCapacity indicates that the CSI volume driver wants pod
-        scheduling to consider the storage capacity that the driver deployment will
-        report by creating CSIStorageCapacity objects with capacity information.
+      * **storageCapacity** ``bool`` - *(optional)* storageCapacity indicates that the CSI volume driver wants pod scheduling to
+        consider the storage capacity that the driver deployment will report by
+        creating CSIStorageCapacity objects with capacity information, if set to true.
         The check can be enabled immediately when deploying a driver. In that case,
         provisioning new volumes with late binding will pause until the driver
         deployment has published some suitable CSIStorageCapacity object.
         Alternatively, the driver can be deployed with the field unset or false and it
         can be flipped later when storage capacity information has been published.
         This field was immutable in Kubernetes <= 1.22 and now is mutable.
-      * **tokenRequests** ``List[TokenRequest]`` - *(optional)* TokenRequests indicates the CSI driver needs pods' service account tokens it
+      * **tokenRequests** ``List[TokenRequest]`` - *(optional)* tokenRequests indicates the CSI driver needs pods' service account tokens it
         is mounting volume for to do necessary authentication. Kubelet will pass the
         tokens in VolumeContext in the CSI NodePublishVolume calls. The CSI driver
         should parse and validate the following VolumeContext:
         "csi.storage.k8s.io/serviceAccount.tokens": {
           "<audience>": {
             "token": <token>,
             "expirationTimestamp": <expiration timestamp in RFC3339>,
@@ -152,23 +154,24 @@
         }
         Note: Audience in each TokenRequest should be different and at most one token
         is empty string. To receive a new token after expiry, RequiresRepublish can be
         used to trigger NodePublishVolume periodically.
       * **volumeLifecycleModes** ``List[str]`` - *(optional)* volumeLifecycleModes defines what kind of volumes this CSI volume driver
         supports. The default if the list is empty is "Persistent", which is the usage
         defined by the CSI specification and implemented in Kubernetes via the usual
-        PV/PVC mechanism. The other mode is "Ephemeral". In this mode, volumes are
-        defined inline inside the pod spec with CSIVolumeSource and their lifecycle is
-        tied to the lifecycle of that pod. A driver has to be aware of this because it
-        is only going to get a NodePublishVolume call for such a volume. For more
-        information about implementing this mode, see
+        PV/PVC mechanism.
+        The other mode is "Ephemeral". In this mode, volumes are defined inline inside
+        the pod spec with CSIVolumeSource and their lifecycle is tied to the lifecycle
+        of that pod. A driver has to be aware of this because it is only going to get
+        a NodePublishVolume call for such a volume.
+        For more information about implementing this mode, see
         https://kubernetes-csi.github.io/docs/ephemeral-local-volumes.html A driver
         can support one or more of these modes and more modes may be added in the
-        future. This field is beta.
-        This field is immutable.
+        future.
+        This field is beta. This field is immutable.
     """
     attachRequired: 'bool' = None
     fsGroupPolicy: 'str' = None
     podInfoOnMount: 'bool' = None
     requiresRepublish: 'bool' = None
     seLinuxMount: 'bool' = None
     storageCapacity: 'bool' = None
@@ -194,31 +197,32 @@
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* metadata.name must be the Kubernetes node name.
+      * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object's metadata. metadata.name must be the Kubernetes node name.
     """
     spec: 'CSINodeSpec'
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
 
 
 @dataclass
 class CSINodeDriver(DataclassDictMixIn):
     """CSINodeDriver holds information about the specification of one CSI driver
       installed on a node
 
       **parameters**
 
-      * **name** ``str`` - This is the name of the CSI driver that this object refers to. This MUST be
-        the same name returned by the CSI GetPluginName() call for that driver.
+      * **name** ``str`` - name represents the name of the CSI driver that this object refers to. This
+        MUST be the same name returned by the CSI GetPluginName() call for that
+        driver.
       * **nodeID** ``str`` - nodeID of the node from the driver point of view. This field enables
         Kubernetes to communicate with storage systems that do not share the same
         nomenclature for nodes. For example, Kubernetes may refer to a given node as
         "node1", but the storage system may refer to the same node as "nodeA". When
         Kubernetes issues a command to the storage system to attach a volume to a
         specific node, it can use this field to refer to the node name using the ID
         that the storage system will understand, e.g. "nodeA" instead of "node1". This
@@ -301,49 +305,50 @@
       compares the MaximumVolumeSize against the requested size of pending volumes
       to filter out unsuitable nodes. If MaximumVolumeSize is unset, it falls back
       to a comparison against the less precise Capacity. If that is also unset, the
       scheduler assumes that capacity is insufficient and tries some other node.
 
       **parameters**
 
-      * **storageClassName** ``str`` - The name of the StorageClass that the reported capacity applies to. It must
-        meet the same requirements as the name of a StorageClass object (non-empty,
-        DNS subdomain). If that object no longer exists, the CSIStorageCapacity object
-        is obsolete and should be removed by its creator. This field is immutable.
+      * **storageClassName** ``str`` - storageClassName represents the name of the StorageClass that the reported
+        capacity applies to. It must meet the same requirements as the name of a
+        StorageClass object (non-empty, DNS subdomain). If that object no longer
+        exists, the CSIStorageCapacity object is obsolete and should be removed by its
+        creator. This field is immutable.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
-      * **capacity** ``resource.Quantity`` - *(optional)* Capacity is the value reported by the CSI driver in its GetCapacityResponse
+      * **capacity** ``resource.Quantity`` - *(optional)* capacity is the value reported by the CSI driver in its GetCapacityResponse
         for a GetCapacityRequest with topology and parameters that match the previous
         fields.
         The semantic is currently (CSI spec 1.2) defined as: The available capacity,
         in bytes, of the storage that can be used to provision volumes. If not set,
         that information is currently unavailable.
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
-      * **maximumVolumeSize** ``resource.Quantity`` - *(optional)* MaximumVolumeSize is the value reported by the CSI driver in its
+      * **maximumVolumeSize** ``resource.Quantity`` - *(optional)* maximumVolumeSize is the value reported by the CSI driver in its
         GetCapacityResponse for a GetCapacityRequest with topology and parameters that
         match the previous fields.
         This is defined since CSI spec 1.4.0 as the largest size that may be used in a
         CreateVolumeRequest.capacity_range.required_bytes field to create a volume
         with the same parameters as those in GetCapacityRequest. The corresponding
         value in the Kubernetes API is ResourceRequirements.Requests in a volume
         claim.
-      * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object's metadata. The name has no particular meaning. It must be be
-        a DNS subdomain (dots allowed, 253 characters). To ensure that there are no
+      * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object's metadata. The name has no particular meaning. It must be a
+        DNS subdomain (dots allowed, 253 characters). To ensure that there are no
         conflicts with other CSI drivers on the cluster, the recommendation is to use
         csisc-<uuid>, a generated name, or a reverse-domain name which ends with the
         unique CSI driver name.
         Objects are namespaced.
         More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **nodeTopology** ``meta_v1.LabelSelector`` - *(optional)* NodeTopology defines which nodes have access to the storage for which capacity
+      * **nodeTopology** ``meta_v1.LabelSelector`` - *(optional)* nodeTopology defines which nodes have access to the storage for which capacity
         was reported. If not set, the storage is not accessible from any node in the
         cluster. If empty, the storage is accessible from all nodes. This field is
         immutable.
     """
     storageClassName: 'str'
     apiVersion: 'str' = None
     capacity: 'resource.Quantity' = None
@@ -355,15 +360,15 @@
 
 @dataclass
 class CSIStorageCapacityList(DataclassDictMixIn):
     """CSIStorageCapacityList is a collection of CSIStorageCapacity objects.
 
       **parameters**
 
-      * **items** ``List[CSIStorageCapacity]`` - Items is the list of CSIStorageCapacity objects.
+      * **items** ``List[CSIStorageCapacity]`` - items is the list of CSIStorageCapacity objects.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
@@ -383,38 +388,39 @@
       PersistentVolumes can be dynamically provisioned.
       
       StorageClasses are non-namespaced; the name of the storage class according to
       etcd is in ObjectMeta.Name.
 
       **parameters**
 
-      * **provisioner** ``str`` - Provisioner indicates the type of the provisioner.
-      * **allowVolumeExpansion** ``bool`` - *(optional)* AllowVolumeExpansion shows whether the storage class allow volume expand
-      * **allowedTopologies** ``List[core_v1.TopologySelectorTerm]`` - *(optional)* Restrict the node topologies where volumes can be dynamically provisioned.
-        Each volume plugin defines its own supported topology specifications. An empty
-        TopologySelectorTerm list means there is no topology restriction. This field
-        is only honored by servers that enable the VolumeScheduling feature.
+      * **provisioner** ``str`` - provisioner indicates the type of the provisioner.
+      * **allowVolumeExpansion** ``bool`` - *(optional)* allowVolumeExpansion shows whether the storage class allow volume expand.
+      * **allowedTopologies** ``List[core_v1.TopologySelectorTerm]`` - *(optional)* allowedTopologies restrict the node topologies where volumes can be
+        dynamically provisioned. Each volume plugin defines its own supported topology
+        specifications. An empty TopologySelectorTerm list means there is no topology
+        restriction. This field is only honored by servers that enable the
+        VolumeScheduling feature.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object's metadata. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **mountOptions** ``List[str]`` - *(optional)* Dynamically provisioned PersistentVolumes of this storage class are created
-        with these mountOptions, e.g. ["ro", "soft"]. Not validated - mount of the PVs
-        will simply fail if one is invalid.
-      * **parameters** ``dict`` - *(optional)* Parameters holds the parameters for the provisioner that should create volumes
+      * **mountOptions** ``List[str]`` - *(optional)* mountOptions controls the mountOptions for dynamically provisioned
+        PersistentVolumes of this storage class. e.g. ["ro", "soft"]. Not validated -
+        mount of the PVs will simply fail if one is invalid.
+      * **parameters** ``dict`` - *(optional)* parameters holds the parameters for the provisioner that should create volumes
         of this storage class.
-      * **reclaimPolicy** ``str`` - *(optional)* Dynamically provisioned PersistentVolumes of this storage class are created
-        with this reclaimPolicy. Defaults to Delete.
-      * **volumeBindingMode** ``str`` - *(optional)* VolumeBindingMode indicates how PersistentVolumeClaims should be provisioned
+      * **reclaimPolicy** ``str`` - *(optional)* reclaimPolicy controls the reclaimPolicy for dynamically provisioned
+        PersistentVolumes of this storage class. Defaults to Delete.
+      * **volumeBindingMode** ``str`` - *(optional)* volumeBindingMode indicates how PersistentVolumeClaims should be provisioned
         and bound.  When unset, VolumeBindingImmediate is used. This field is only
         honored by servers that enable the VolumeScheduling feature.
     """
     provisioner: 'str'
     allowVolumeExpansion: 'bool' = None
     allowedTopologies: 'List[core_v1.TopologySelectorTerm]' = None
     apiVersion: 'str' = None
@@ -428,15 +434,15 @@
 
 @dataclass
 class StorageClassList(DataclassDictMixIn):
     """StorageClassList is a collection of storage classes.
 
       **parameters**
 
-      * **items** ``List[StorageClass]`` - Items is the list of StorageClasses
+      * **items** ``List[StorageClass]`` - items is the list of StorageClasses
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
@@ -452,17 +458,17 @@
 
 @dataclass
 class TokenRequest(DataclassDictMixIn):
     """TokenRequest contains parameters of a service account token.
 
       **parameters**
 
-      * **audience** ``str`` - Audience is the intended audience of the token in "TokenRequestSpec". It will
+      * **audience** ``str`` - audience is the intended audience of the token in "TokenRequestSpec". It will
         default to the audiences of kube apiserver.
-      * **expirationSeconds** ``int`` - *(optional)* ExpirationSeconds is the duration of validity of the token in
+      * **expirationSeconds** ``int`` - *(optional)* expirationSeconds is the duration of validity of the token in
         "TokenRequestSpec". It has the same default value of "ExpirationSeconds" in
         "TokenRequestSpec".
     """
     audience: 'str'
     expirationSeconds: 'int' = None
 
 
@@ -471,43 +477,43 @@
     """VolumeAttachment captures the intent to attach or detach the specified volume
       to/from the specified node.
       
       VolumeAttachment objects are non-namespaced.
 
       **parameters**
 
-      * **spec** ``VolumeAttachmentSpec`` - Specification of the desired attach/detach volume behavior. Populated by the
-        Kubernetes system.
+      * **spec** ``VolumeAttachmentSpec`` - spec represents specification of the desired attach/detach volume behavior.
+        Populated by the Kubernetes system.
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **metadata** ``meta_v1.ObjectMeta`` - *(optional)* Standard object metadata. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
-      * **status** ``VolumeAttachmentStatus`` - *(optional)* Status of the VolumeAttachment request. Populated by the entity completing the
-        attach or detach operation, i.e. the external-attacher.
+      * **status** ``VolumeAttachmentStatus`` - *(optional)* status represents status of the VolumeAttachment request. Populated by the
+        entity completing the attach or detach operation, i.e. the external-attacher.
     """
     spec: 'VolumeAttachmentSpec'
     apiVersion: 'str' = None
     kind: 'str' = None
     metadata: 'meta_v1.ObjectMeta' = None
     status: 'VolumeAttachmentStatus' = None
 
 
 @dataclass
 class VolumeAttachmentList(DataclassDictMixIn):
     """VolumeAttachmentList is a collection of VolumeAttachment objects.
 
       **parameters**
 
-      * **items** ``List[VolumeAttachment]`` - Items is the list of VolumeAttachments
+      * **items** ``List[VolumeAttachment]`` - items is the list of VolumeAttachments
       * **apiVersion** ``str`` - *(optional)* APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
       * **kind** ``str`` - *(optional)* Kind is a string value representing the REST resource this object represents.
         Servers may infer this from the endpoint the client submits requests to.
         Cannot be updated. In CamelCase. More info:
@@ -530,83 +536,85 @@
       **parameters**
 
       * **inlineVolumeSpec** ``core_v1.PersistentVolumeSpec`` - *(optional)* inlineVolumeSpec contains all the information necessary to attach a persistent
         volume defined by a pod's inline VolumeSource. This field is populated only
         for the CSIMigration feature. It contains translated fields from a pod's
         inline VolumeSource to a PersistentVolumeSpec. This field is beta-level and is
         only honored by servers that enabled the CSIMigration feature.
-      * **persistentVolumeName** ``str`` - *(optional)* Name of the persistent volume to attach.
+      * **persistentVolumeName** ``str`` - *(optional)* persistentVolumeName represents the name of the persistent volume to attach.
     """
     inlineVolumeSpec: 'core_v1.PersistentVolumeSpec' = None
     persistentVolumeName: 'str' = None
 
 
 @dataclass
 class VolumeAttachmentSpec(DataclassDictMixIn):
     """VolumeAttachmentSpec is the specification of a VolumeAttachment request.
 
       **parameters**
 
-      * **attacher** ``str`` - Attacher indicates the name of the volume driver that MUST handle this
+      * **attacher** ``str`` - attacher indicates the name of the volume driver that MUST handle this
         request. This is the name returned by GetPluginName().
-      * **nodeName** ``str`` - The node that the volume should be attached to.
-      * **source** ``VolumeAttachmentSource`` - Source represents the volume that should be attached.
+      * **nodeName** ``str`` - nodeName represents the node that the volume should be attached to.
+      * **source** ``VolumeAttachmentSource`` - source represents the volume that should be attached.
     """
     attacher: 'str'
     nodeName: 'str'
     source: 'VolumeAttachmentSource'
 
 
 @dataclass
 class VolumeAttachmentStatus(DataclassDictMixIn):
     """VolumeAttachmentStatus is the status of a VolumeAttachment request.
 
       **parameters**
 
-      * **attached** ``bool`` - Indicates the volume is successfully attached. This field must only be set by
-        the entity completing the attach operation, i.e. the external-attacher.
-      * **attachError** ``VolumeError`` - *(optional)* The last error encountered during attach operation, if any. This field must
-        only be set by the entity completing the attach operation, i.e. the
+      * **attached** ``bool`` - attached indicates the volume is successfully attached. This field must only
+        be set by the entity completing the attach operation, i.e. the
         external-attacher.
-      * **attachmentMetadata** ``dict`` - *(optional)* Upon successful attach, this field is populated with any information returned
-        by the attach operation that must be passed into subsequent WaitForAttach or
-        Mount calls. This field must only be set by the entity completing the attach
+      * **attachError** ``VolumeError`` - *(optional)* attachError represents the last error encountered during attach operation, if
+        any. This field must only be set by the entity completing the attach
+        operation, i.e. the external-attacher.
+      * **attachmentMetadata** ``dict`` - *(optional)* attachmentMetadata is populated with any information returned by the attach
+        operation, upon successful attach, that must be passed into subsequent
+        WaitForAttach or Mount calls. This field must only be set by the entity
+        completing the attach operation, i.e. the external-attacher.
+      * **detachError** ``VolumeError`` - *(optional)* detachError represents the last error encountered during detach operation, if
+        any. This field must only be set by the entity completing the detach
         operation, i.e. the external-attacher.
-      * **detachError** ``VolumeError`` - *(optional)* The last error encountered during detach operation, if any. This field must
-        only be set by the entity completing the detach operation, i.e. the
-        external-attacher.
     """
     attached: 'bool'
     attachError: 'VolumeError' = None
     attachmentMetadata: 'dict' = None
     detachError: 'VolumeError' = None
 
 
 @dataclass
 class VolumeError(DataclassDictMixIn):
     """VolumeError captures an error encountered during a volume operation.
 
       **parameters**
 
-      * **message** ``str`` - *(optional)* String detailing the error encountered during Attach or Detach operation. This
-        string may be logged, so it should not contain sensitive information.
-      * **time** ``meta_v1.Time`` - *(optional)* Time the error was encountered.
+      * **message** ``str`` - *(optional)* message represents the error encountered during Attach or Detach operation.
+        This string may be logged, so it should not contain sensitive information.
+      * **time** ``meta_v1.Time`` - *(optional)* time represents the time the error was encountered.
     """
     message: 'str' = None
     time: 'meta_v1.Time' = None
 
 
 @dataclass
 class VolumeNodeResources(DataclassDictMixIn):
     """VolumeNodeResources is a set of resource limits for scheduling of volumes.
 
       **parameters**
 
-      * **count** ``int`` - *(optional)* Maximum number of unique volumes managed by the CSI driver that can be used on
-        a node. A volume that is both attached and mounted on a node is considered to
-        be used once, not twice. The same rule applies for a unique volume that is
-        shared among multiple pods on the same node. If this field is not specified,
-        then the supported number of volumes on this node is unbounded.
+      * **count** ``int`` - *(optional)* count indicates the maximum number of unique volumes managed by the CSI driver
+        that can be used on a node. A volume that is both attached and mounted on a
+        node is considered to be used once, not twice. The same rule applies for a
+        unique volume that is shared among multiple pods on the same node. If this
+        field is not specified, then the supported number of volumes on this node is
+        unbounded.
     """
     count: 'int' = None
```

### Comparing `lightkube-models-1.26.0.4/lightkube/models/version.py` & `lightkube-models-1.27.1.4/lightkube/models/version.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/admissionregistration_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/admissionregistration_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/admissionregistration_v1alpha1.py` & `lightkube-models-1.27.1.4/lightkube/resources/admissionregistration_v1alpha1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,45 @@
 # autogenerated module
 from typing import ClassVar
 
 from ..core import resource as res
 from ..models import admissionregistration_v1alpha1 as m_admissionregistration_v1alpha1
 
 
+class ValidatingAdmissionPolicyStatus(res.GlobalSubResource, m_admissionregistration_v1alpha1.ValidatingAdmissionPolicy):
+    """* **Extends**: ``models.admissionregistration_v1alpha1.ValidatingAdmissionPolicy``
+       * **Type**: Global Resource
+       * **Accepted client methods**: `get`, `patch`, `replace`
+    """
+    _api_info = res.ApiInfo(
+        resource=res.ResourceDef('admissionregistration.k8s.io', 'v1alpha1', 'ValidatingAdmissionPolicy'),
+        parent=res.ResourceDef('admissionregistration.k8s.io', 'v1alpha1', 'ValidatingAdmissionPolicy'),
+        plural='validatingadmissionpolicies',
+        verbs=['get', 'patch', 'put'],
+        action='status',
+    )
+
+
 class ValidatingAdmissionPolicy(res.GlobalResource, m_admissionregistration_v1alpha1.ValidatingAdmissionPolicy):
     """* **Extends**: ``models.admissionregistration_v1alpha1.ValidatingAdmissionPolicy``
        * **Type**: Global Resource
        * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list`, `patch`, `create`, `replace`, `watch`
+
+       **Subresources**:
+
+       * **Status**: ``ValidatingAdmissionPolicyStatus``
     """
     _api_info = res.ApiInfo(
         resource=res.ResourceDef('admissionregistration.k8s.io', 'v1alpha1', 'ValidatingAdmissionPolicy'),
         plural='validatingadmissionpolicies',
         verbs=['delete', 'deletecollection', 'get', 'list', 'patch', 'post', 'put', 'watch'],
     )
 
+    Status: ClassVar = ValidatingAdmissionPolicyStatus
+
 
 class ValidatingAdmissionPolicyBinding(res.GlobalResource, m_admissionregistration_v1alpha1.ValidatingAdmissionPolicyBinding):
     """* **Extends**: ``models.admissionregistration_v1alpha1.ValidatingAdmissionPolicyBinding``
        * **Type**: Global Resource
        * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list`, `patch`, `create`, `replace`, `watch`
     """
     _api_info = res.ApiInfo(
```

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/apiextensions_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/apiextensions_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/apiregistration_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/apiregistration_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/apps_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/apps_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/authentication_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/authentication_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/authentication_v1alpha1.py` & `lightkube-models-1.27.1.4/lightkube/resources/authentication_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/authorization_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/authorization_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/autoscaling_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/autoscaling_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/autoscaling_v2.py` & `lightkube-models-1.27.1.4/lightkube/resources/autoscaling_v2.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/batch_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/batch_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/certificates_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/certificates_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/coordination_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/coordination_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/core_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/core_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/discovery_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/discovery_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/events_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/events_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/flowcontrol_apiserver_v1beta2.py` & `lightkube-models-1.27.1.4/lightkube/resources/flowcontrol_apiserver_v1beta2.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/flowcontrol_apiserver_v1beta3.py` & `lightkube-models-1.27.1.4/lightkube/resources/flowcontrol_apiserver_v1beta3.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/internal_apiserver_v1alpha1.py` & `lightkube-models-1.27.1.4/lightkube/resources/internal_apiserver_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/networking_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/networking_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/networking_v1alpha1.py` & `lightkube-models-1.27.1.4/lightkube/resources/networking_v1alpha1.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,7 +12,19 @@
     """
     _api_info = res.ApiInfo(
         resource=res.ResourceDef('networking.k8s.io', 'v1alpha1', 'ClusterCIDR'),
         plural='clustercidrs',
         verbs=['delete', 'deletecollection', 'get', 'list', 'patch', 'post', 'put', 'watch'],
     )
 
+
+class IPAddress(res.GlobalResource, m_networking_v1alpha1.IPAddress):
+    """* **Extends**: ``models.networking_v1alpha1.IPAddress``
+       * **Type**: Global Resource
+       * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list`, `patch`, `create`, `replace`, `watch`
+    """
+    _api_info = res.ApiInfo(
+        resource=res.ResourceDef('networking.k8s.io', 'v1alpha1', 'IPAddress'),
+        plural='ipaddresses',
+        verbs=['delete', 'deletecollection', 'get', 'list', 'patch', 'post', 'put', 'watch'],
+    )
+
```

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/node_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/node_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/policy_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/policy_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/rbac_authorization_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/rbac_authorization_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/resource_v1alpha1.py` & `lightkube-models-1.27.1.4/lightkube/resources/resource_v1alpha2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 # autogenerated module
 from typing import ClassVar
 
 from ..core import resource as res
-from ..models import resource_v1alpha1 as m_resource_v1alpha1
+from ..models import resource_v1alpha2 as m_resource_v1alpha2
 
 
-class PodSchedulingStatus(res.NamespacedSubResource, m_resource_v1alpha1.PodScheduling):
-    """* **Extends**: ``models.resource_v1alpha1.PodScheduling``
+class PodSchedulingContextStatus(res.NamespacedSubResource, m_resource_v1alpha2.PodSchedulingContext):
+    """* **Extends**: ``models.resource_v1alpha2.PodSchedulingContext``
        * **Type**: Namespaced Resource
        * **Accepted client methods**: `get`, `patch`, `replace`
     """
     _api_info = res.ApiInfo(
-        resource=res.ResourceDef('resource.k8s.io', 'v1alpha1', 'PodScheduling'),
-        parent=res.ResourceDef('resource.k8s.io', 'v1alpha1', 'PodScheduling'),
-        plural='podschedulings',
+        resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'PodSchedulingContext'),
+        parent=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'PodSchedulingContext'),
+        plural='podschedulingcontexts',
         verbs=['get', 'patch', 'put'],
         action='status',
     )
 
 
-class PodScheduling(res.NamespacedResourceG, m_resource_v1alpha1.PodScheduling):
-    """* **Extends**: ``models.resource_v1alpha1.PodScheduling``
+class PodSchedulingContext(res.NamespacedResourceG, m_resource_v1alpha2.PodSchedulingContext):
+    """* **Extends**: ``models.resource_v1alpha2.PodSchedulingContext``
        * **Type**: Namespaced Resource
        * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list` all, `watch` all, `list`, `patch`, `create`, `replace`, `watch`
 
        **Subresources**:
 
-       * **Status**: ``PodSchedulingStatus``
+       * **Status**: ``PodSchedulingContextStatus``
     """
     _api_info = res.ApiInfo(
-        resource=res.ResourceDef('resource.k8s.io', 'v1alpha1', 'PodScheduling'),
-        plural='podschedulings',
+        resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'PodSchedulingContext'),
+        plural='podschedulingcontexts',
         verbs=['delete', 'deletecollection', 'get', 'global_list', 'global_watch', 'list', 'patch', 'post', 'put', 'watch'],
     )
 
-    Status: ClassVar = PodSchedulingStatus
+    Status: ClassVar = PodSchedulingContextStatus
 
 
-class ResourceClaimStatus(res.NamespacedSubResource, m_resource_v1alpha1.ResourceClaim):
-    """* **Extends**: ``models.resource_v1alpha1.ResourceClaim``
+class ResourceClaimStatus(res.NamespacedSubResource, m_resource_v1alpha2.ResourceClaim):
+    """* **Extends**: ``models.resource_v1alpha2.ResourceClaim``
        * **Type**: Namespaced Resource
        * **Accepted client methods**: `get`, `patch`, `replace`
     """
     _api_info = res.ApiInfo(
-        resource=res.ResourceDef('resource.k8s.io', 'v1alpha1', 'ResourceClaim'),
-        parent=res.ResourceDef('resource.k8s.io', 'v1alpha1', 'ResourceClaim'),
+        resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceClaim'),
+        parent=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceClaim'),
         plural='resourceclaims',
         verbs=['get', 'patch', 'put'],
         action='status',
     )
 
 
-class ResourceClaim(res.NamespacedResourceG, m_resource_v1alpha1.ResourceClaim):
-    """* **Extends**: ``models.resource_v1alpha1.ResourceClaim``
+class ResourceClaim(res.NamespacedResourceG, m_resource_v1alpha2.ResourceClaim):
+    """* **Extends**: ``models.resource_v1alpha2.ResourceClaim``
        * **Type**: Namespaced Resource
        * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list` all, `watch` all, `list`, `patch`, `create`, `replace`, `watch`
 
        **Subresources**:
 
        * **Status**: ``ResourceClaimStatus``
     """
     _api_info = res.ApiInfo(
-        resource=res.ResourceDef('resource.k8s.io', 'v1alpha1', 'ResourceClaim'),
+        resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceClaim'),
         plural='resourceclaims',
         verbs=['delete', 'deletecollection', 'get', 'global_list', 'global_watch', 'list', 'patch', 'post', 'put', 'watch'],
     )
 
     Status: ClassVar = ResourceClaimStatus
 
 
-class ResourceClaimTemplate(res.NamespacedResourceG, m_resource_v1alpha1.ResourceClaimTemplate):
-    """* **Extends**: ``models.resource_v1alpha1.ResourceClaimTemplate``
+class ResourceClaimTemplate(res.NamespacedResourceG, m_resource_v1alpha2.ResourceClaimTemplate):
+    """* **Extends**: ``models.resource_v1alpha2.ResourceClaimTemplate``
        * **Type**: Namespaced Resource
        * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list` all, `watch` all, `list`, `patch`, `create`, `replace`, `watch`
     """
     _api_info = res.ApiInfo(
-        resource=res.ResourceDef('resource.k8s.io', 'v1alpha1', 'ResourceClaimTemplate'),
+        resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceClaimTemplate'),
         plural='resourceclaimtemplates',
         verbs=['delete', 'deletecollection', 'get', 'global_list', 'global_watch', 'list', 'patch', 'post', 'put', 'watch'],
     )
 
 
-class ResourceClass(res.GlobalResource, m_resource_v1alpha1.ResourceClass):
-    """* **Extends**: ``models.resource_v1alpha1.ResourceClass``
+class ResourceClass(res.GlobalResource, m_resource_v1alpha2.ResourceClass):
+    """* **Extends**: ``models.resource_v1alpha2.ResourceClass``
        * **Type**: Global Resource
        * **Accepted client methods**: `delete`, `deletecollection`, `get`, `list`, `patch`, `create`, `replace`, `watch`
     """
     _api_info = res.ApiInfo(
-        resource=res.ResourceDef('resource.k8s.io', 'v1alpha1', 'ResourceClass'),
+        resource=res.ResourceDef('resource.k8s.io', 'v1alpha2', 'ResourceClass'),
         plural='resourceclasses',
         verbs=['delete', 'deletecollection', 'get', 'list', 'patch', 'post', 'put', 'watch'],
     )
```

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/scheduling_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/scheduling_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube/resources/storage_v1.py` & `lightkube-models-1.27.1.4/lightkube/resources/storage_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.26.0.4/lightkube_models.egg-info/PKG-INFO` & `lightkube-models-1.27.1.4/lightkube_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightkube-models
-Version: 1.26.0.4
+Version: 1.27.1.4
 Summary: Models and Resources for lightkube module
 Home-page: https://github.com/gtsystem/lightkube-models
 Author: Giuseppe Tribulato
 Author-email: gtsystem@gmail.com
 License: Apache Software License
 Description: # lightkube-models
```

### Comparing `lightkube-models-1.26.0.4/lightkube_models.egg-info/SOURCES.txt` & `lightkube-models-1.27.1.4/lightkube_models.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,64 +6,66 @@
 lightkube/models/admissionregistration_v1alpha1.py
 lightkube/models/apiextensions_v1.py
 lightkube/models/apiregistration_v1.py
 lightkube/models/apiserverinternal_v1alpha1.py
 lightkube/models/apps_v1.py
 lightkube/models/authentication_v1.py
 lightkube/models/authentication_v1alpha1.py
+lightkube/models/authentication_v1beta1.py
 lightkube/models/authorization_v1.py
 lightkube/models/autoscaling_v1.py
 lightkube/models/autoscaling_v2.py
 lightkube/models/batch_v1.py
 lightkube/models/certificates_v1.py
+lightkube/models/certificates_v1alpha1.py
 lightkube/models/coordination_v1.py
 lightkube/models/core_v1.py
 lightkube/models/discovery_v1.py
 lightkube/models/events_v1.py
 lightkube/models/flowcontrol_v1beta2.py
 lightkube/models/flowcontrol_v1beta3.py
 lightkube/models/meta_v1.py
 lightkube/models/networking_v1.py
 lightkube/models/networking_v1alpha1.py
 lightkube/models/node_v1.py
 lightkube/models/policy_v1.py
 lightkube/models/rbac_v1.py
 lightkube/models/resource.py
-lightkube/models/resource_v1alpha1.py
+lightkube/models/resource_v1alpha2.py
 lightkube/models/runtime.py
 lightkube/models/scheduling_v1.py
 lightkube/models/storage_v1.py
-lightkube/models/storage_v1beta1.py
 lightkube/models/util_intstr.py
 lightkube/models/version.py
 lightkube/resources/admissionregistration_v1.py
 lightkube/resources/admissionregistration_v1alpha1.py
 lightkube/resources/apiextensions_v1.py
 lightkube/resources/apiregistration_v1.py
 lightkube/resources/apps_v1.py
 lightkube/resources/authentication_v1.py
 lightkube/resources/authentication_v1alpha1.py
+lightkube/resources/authentication_v1beta1.py
 lightkube/resources/authorization_v1.py
 lightkube/resources/autoscaling_v1.py
 lightkube/resources/autoscaling_v2.py
 lightkube/resources/batch_v1.py
 lightkube/resources/certificates_v1.py
+lightkube/resources/certificates_v1alpha1.py
 lightkube/resources/coordination_v1.py
 lightkube/resources/core_v1.py
 lightkube/resources/discovery_v1.py
 lightkube/resources/events_v1.py
 lightkube/resources/flowcontrol_apiserver_v1beta2.py
 lightkube/resources/flowcontrol_apiserver_v1beta3.py
 lightkube/resources/internal_apiserver_v1alpha1.py
 lightkube/resources/networking_v1.py
 lightkube/resources/networking_v1alpha1.py
 lightkube/resources/node_v1.py
 lightkube/resources/policy_v1.py
 lightkube/resources/rbac_authorization_v1.py
-lightkube/resources/resource_v1alpha1.py
+lightkube/resources/resource_v1alpha2.py
 lightkube/resources/scheduling_v1.py
 lightkube/resources/storage_v1.py
-lightkube/resources/storage_v1beta1.py
 lightkube_models.egg-info/PKG-INFO
 lightkube_models.egg-info/SOURCES.txt
 lightkube_models.egg-info/dependency_links.txt
 lightkube_models.egg-info/top_level.txt
```

### Comparing `lightkube-models-1.26.0.4/setup.py` & `lightkube-models-1.27.1.4/setup.py`

 * *Files identical despite different names*

