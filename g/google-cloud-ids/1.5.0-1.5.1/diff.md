# Comparing `tmp/google-cloud-ids-1.5.0.tar.gz` & `tmp/google-cloud-ids-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-ids-1.5.0.tar", last modified: Fri Feb 24 01:14:26 2023, max compression
+gzip compressed data, was "google-cloud-ids-1.5.1.tar", last modified: Fri Apr 21 13:52:32 2023, max compression
```

## Comparing `google-cloud-ids-1.5.0.tar` & `google-cloud-ids-1.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.771891 google-cloud-ids-1.5.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4577 2023-02-24 01:14:26.771891 google-cloud-ids-1.5.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3673 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.763896 google-cloud-ids-1.5.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.763896 google-cloud-ids-1.5.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.763896 google-cloud-ids-1.5.0/google/cloud/ids/
--rw-rw-r--   0 root         (0)     1003     1292 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.767894 google-cloud-ids-1.5.0/google/cloud/ids_v1/
--rw-rw-r--   0 root         (0)     1003     1193 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2068 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.767894 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.767894 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/
--rw-rw-r--   0 root         (0)     1003      725 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/__init__.py
--rw-rw-r--   0 root         (0)     1003    28490 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/async_client.py
--rw-rw-r--   0 root         (0)     1003    37521 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/client.py
--rw-rw-r--   0 root         (0)     1003     5614 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.767894 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8104 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15455 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15775 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    28427 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.767894 google-cloud-ids-1.5.0/google/cloud/ids_v1/types/
--rw-rw-r--   0 root         (0)     1003      986 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12436 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/google/cloud/ids_v1/types/ids.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.767894 google-cloud-ids-1.5.0/google_cloud_ids.egg-info/
--rw-r--r--   0 root         (0)     1003     4577 2023-02-24 01:14:26.000000 google-cloud-ids-1.5.0/google_cloud_ids.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1269 2023-02-24 01:14:26.000000 google-cloud-ids-1.5.0/google_cloud_ids.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-24 01:14:26.000000 google-cloud-ids-1.5.0/google_cloud_ids.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-02-24 01:14:26.000000 google-cloud-ids-1.5.0/google_cloud_ids.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-24 01:14:26.000000 google-cloud-ids-1.5.0/google_cloud_ids.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-02-24 01:14:26.000000 google-cloud-ids-1.5.0/google_cloud_ids.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-02-24 01:14:26.000000 google-cloud-ids-1.5.0/google_cloud_ids.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-02-24 01:14:26.771891 google-cloud-ids-1.5.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2905 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.767894 google-cloud-ids-1.5.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.767894 google-cloud-ids-1.5.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.771891 google-cloud-ids-1.5.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 01:14:26.771891 google-cloud-ids-1.5.0/tests/unit/gapic/ids_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/tests/unit/gapic/ids_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   135027 2023-02-24 01:12:07.000000 google-cloud-ids-1.5.0/tests/unit/gapic/ids_v1/test_ids.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4817 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3904 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.921610 google-cloud-ids-1.5.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.921610 google-cloud-ids-1.5.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids/
+-rw-rw-r--   0 root         (0)     1003     1292 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids_v1/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2068 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/
+-rw-rw-r--   0 root         (0)     1003      725 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28490 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37521 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/client.py
+-rw-rw-r--   0 root         (0)     1003     5614 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8104 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15455 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15775 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    28432 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.925610 google-cloud-ids-1.5.1/google/cloud/ids_v1/types/
+-rw-rw-r--   0 root         (0)     1003      986 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12472 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/google/cloud/ids_v1/types/ids.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/
+-rw-r--r--   0 root         (0)     1003     4817 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1269 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-21 13:52:32.000000 google-cloud-ids-1.5.1/google_cloud_ids.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2914 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-21 13:52:32.929609 google-cloud-ids-1.5.1/tests/unit/gapic/ids_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/tests/unit/gapic/ids_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   135027 2023-04-21 13:50:08.000000 google-cloud-ids-1.5.1/tests/unit/gapic/ids_v1/test_ids.py
```

### Comparing `google-cloud-ids-1.5.0/LICENSE` & `google-cloud-ids-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/MANIFEST.in` & `google-cloud-ids-1.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/PKG-INFO` & `google-cloud-ids-1.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-ids
-Version: 1.5.0
+Version: 1.5.1
 Summary: Google Cloud Ids API client library
-Home-page: https://github.com/googleapis/python-ids
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Cloud IDS API
-===============================
+Python Client for Cloud IDS
+===========================
 
 |stable| |pypi| |versions|
 
-`Cloud IDS API`_:  monitors your networks, and it alerts you when it detects malicious activity. Cloud IDS is powered by Palo Alto Networks.
+`Cloud IDS`_: Cloud IDS is an intrusion detection service that provides threat detection for intrusions, malware, spyware, and command-and-control attacks on your network. Cloud IDS works by creating a Google-managed peered network with mirrored VMs. Traffic in the peered network is mirrored, and then inspected by Palo Alto Networks threat protection technologies to provide advanced threat detection.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-ids.svg
    :target: https://pypi.org/project/google-cloud-ids/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-ids.svg
    :target: https://pypi.org/project/google-cloud-ids/
-.. _Cloud IDS API: https://cloud.google.com/intrusion-detection-system/
+.. _Cloud IDS: https://cloud.google.com/intrusion-detection-system/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/ids/latest
 .. _Product Documentation:  https://cloud.google.com/intrusion-detection-system/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud IDS API.`_
+3. `Enable the Cloud IDS.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud IDS API.:  https://cloud.google.com/intrusion-detection-system/
+.. _Enable the Cloud IDS.:  https://cloud.google.com/intrusion-detection-system/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-ids
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud IDS API
+-  Read the `Client Library Documentation`_ for Cloud IDS
    to see other available methods on the client.
--  Read the `Cloud IDS API Product documentation`_ to learn
+-  Read the `Cloud IDS Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud IDS API Product documentation:  https://cloud.google.com/intrusion-detection-system/
+.. _Cloud IDS Product documentation:  https://cloud.google.com/intrusion-detection-system/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-ids-1.5.0/README.rst` & `google-cloud-ids-1.5.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud IDS API
-===============================
+Python Client for Cloud IDS
+===========================
 
 |stable| |pypi| |versions|
 
-`Cloud IDS API`_:  monitors your networks, and it alerts you when it detects malicious activity. Cloud IDS is powered by Palo Alto Networks.
+`Cloud IDS`_: Cloud IDS is an intrusion detection service that provides threat detection for intrusions, malware, spyware, and command-and-control attacks on your network. Cloud IDS works by creating a Google-managed peered network with mirrored VMs. Traffic in the peered network is mirrored, and then inspected by Palo Alto Networks threat protection technologies to provide advanced threat detection.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-ids.svg
    :target: https://pypi.org/project/google-cloud-ids/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-ids.svg
    :target: https://pypi.org/project/google-cloud-ids/
-.. _Cloud IDS API: https://cloud.google.com/intrusion-detection-system/
+.. _Cloud IDS: https://cloud.google.com/intrusion-detection-system/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/ids/latest
 .. _Product Documentation:  https://cloud.google.com/intrusion-detection-system/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud IDS API.`_
+3. `Enable the Cloud IDS.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud IDS API.:  https://cloud.google.com/intrusion-detection-system/
+.. _Enable the Cloud IDS.:  https://cloud.google.com/intrusion-detection-system/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-ids
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud IDS API
+-  Read the `Client Library Documentation`_ for Cloud IDS
    to see other available methods on the client.
--  Read the `Cloud IDS API Product documentation`_ to learn
+-  Read the `Cloud IDS Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud IDS API Product documentation:  https://cloud.google.com/intrusion-detection-system/
+.. _Cloud IDS Product documentation:  https://cloud.google.com/intrusion-detection-system/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids/__init__.py` & `google-cloud-ids-1.5.1/google/cloud/ids/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids/gapic_version.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.0"  # {x-release-please-version}
+from .async_client import IDSAsyncClient
+from .client import IDSClient
+
+__all__ = (
+    "IDSClient",
+    "IDSAsyncClient",
+)
```

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/__init__.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/gapic_metadata.json` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/gapic_version.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.0"  # {x-release-please-version}
```

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/services/__init__.py` & `google-cloud-ids-1.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/__init__.py` & `google-cloud-ids-1.5.1/tests/unit/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .async_client import IDSAsyncClient
-from .client import IDSClient
-
-__all__ = (
-    "IDSClient",
-    "IDSAsyncClient",
-)
```

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/async_client.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/client.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/pagers.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/__init__.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/base.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/grpc.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/grpc_asyncio.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/services/ids/transports/rest.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/services/ids/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import dataclasses
 import json  # type: ignore
 import re
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import (
     gapic_v1,
     operations_v1,
     path_template,
     rest_helpers,
@@ -342,15 +342,15 @@
         # Return the client from cache.
         return self._operations_client
 
     class _CreateEndpoint(IDSRestStub):
         def __hash__(self):
             return hash("CreateEndpoint")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
             "endpointId": "",
         }
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
@@ -440,15 +440,15 @@
             resp = self._interceptor.post_create_endpoint(resp)
             return resp
 
     class _DeleteEndpoint(IDSRestStub):
         def __hash__(self):
             return hash("DeleteEndpoint")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -527,15 +527,15 @@
             resp = self._interceptor.post_delete_endpoint(resp)
             return resp
 
     class _GetEndpoint(IDSRestStub):
         def __hash__(self):
             return hash("GetEndpoint")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -617,15 +617,15 @@
             resp = self._interceptor.post_get_endpoint(resp)
             return resp
 
     class _ListEndpoints(IDSRestStub):
         def __hash__(self):
             return hash("ListEndpoints")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
```

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/types/__init__.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/google/cloud/ids_v1/types/ids.py` & `google-cloud-ids-1.5.1/google/cloud/ids_v1/types/ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.ids.v1",
```

### Comparing `google-cloud-ids-1.5.0/google_cloud_ids.egg-info/PKG-INFO` & `google-cloud-ids-1.5.1/google_cloud_ids.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-ids
-Version: 1.5.0
+Version: 1.5.1
 Summary: Google Cloud Ids API client library
-Home-page: https://github.com/googleapis/python-ids
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Cloud IDS API
-===============================
+Python Client for Cloud IDS
+===========================
 
 |stable| |pypi| |versions|
 
-`Cloud IDS API`_:  monitors your networks, and it alerts you when it detects malicious activity. Cloud IDS is powered by Palo Alto Networks.
+`Cloud IDS`_: Cloud IDS is an intrusion detection service that provides threat detection for intrusions, malware, spyware, and command-and-control attacks on your network. Cloud IDS works by creating a Google-managed peered network with mirrored VMs. Traffic in the peered network is mirrored, and then inspected by Palo Alto Networks threat protection technologies to provide advanced threat detection.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-ids.svg
    :target: https://pypi.org/project/google-cloud-ids/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-ids.svg
    :target: https://pypi.org/project/google-cloud-ids/
-.. _Cloud IDS API: https://cloud.google.com/intrusion-detection-system/
+.. _Cloud IDS: https://cloud.google.com/intrusion-detection-system/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/ids/latest
 .. _Product Documentation:  https://cloud.google.com/intrusion-detection-system/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud IDS API.`_
+3. `Enable the Cloud IDS.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud IDS API.:  https://cloud.google.com/intrusion-detection-system/
+.. _Enable the Cloud IDS.:  https://cloud.google.com/intrusion-detection-system/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-ids
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud IDS API
+-  Read the `Client Library Documentation`_ for Cloud IDS
    to see other available methods on the client.
--  Read the `Cloud IDS API Product documentation`_ to learn
+-  Read the `Cloud IDS Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud IDS API Product documentation:  https://cloud.google.com/intrusion-detection-system/
+.. _Cloud IDS Product documentation:  https://cloud.google.com/intrusion-detection-system/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-ids-1.5.0/google_cloud_ids.egg-info/SOURCES.txt` & `google-cloud-ids-1.5.1/google_cloud_ids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/setup.py` & `google-cloud-ids-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-ids"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-ids-1.5.0/tests/__init__.py` & `google-cloud-ids-1.5.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/tests/unit/__init__.py` & `google-cloud-ids-1.5.1/tests/unit/gapic/ids_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ids-1.5.0/tests/unit/gapic/ids_v1/test_ids.py` & `google-cloud-ids-1.5.1/tests/unit/gapic/ids_v1/test_ids.py`

 * *Files identical despite different names*

