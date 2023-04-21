# Comparing `tmp/oms-mqclient-1.2.0.tar.gz` & `tmp/oms-mqclient-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-1.2.0.tar", last modified: Wed Apr  5 16:33:06 2023, max compression
+gzip compressed data, was "oms-mqclient-2.0.0.tar", last modified: Fri Apr 21 20:01:30 2023, max compression
```

## Comparing `oms-mqclient-1.2.0.tar` & `oms-mqclient-2.0.0.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:33:06.778350 oms-mqclient-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2728 2023-04-05 16:33:06.778350 oms-mqclient-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1377 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:33:06.774351 oms-mqclient-1.2.0/mqclient/
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-05 16:33:03.000000 oms-mqclient-1.2.0/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5676 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:33:06.774351 oms-mqclient-1.2.0/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12343 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    15070 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/broker_clients/gcp.py
--rw-r--r--   0 root         (0) root         (0)    12296 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    15440 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)      213 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    17025 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:33:06.774351 oms-mqclient-1.2.0/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2728 2023-04-05 16:33:06.000000 oms-mqclient-1.2.0/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1177 2023-04-05 16:33:06.000000 oms-mqclient-1.2.0/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 16:33:06.000000 oms-mqclient-1.2.0/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-05 16:33:06.000000 oms-mqclient-1.2.0/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-05 16:33:06.000000 oms-mqclient-1.2.0/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2869 2023-04-05 16:33:06.782350 oms-mqclient-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:33:06.770351 oms-mqclient-1.2.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:33:06.778350 oms-mqclient-1.2.0/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7026 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    20662 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    18702 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:33:06.778350 oms-mqclient-1.2.0/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)      838 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/integrate/test_gcp.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:33:06.778350 oms-mqclient-1.2.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:33:06.778350 oms-mqclient-1.2.0/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:33:06.778350 oms-mqclient-1.2.0/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8202 2023-04-05 16:33:02.000000 oms-mqclient-1.2.0/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.664924 oms-mqclient-2.0.0/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-21 20:01:28.000000 oms-mqclient-2.0.0/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5676 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.664924 oms-mqclient-2.0.0/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12343 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    12296 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    15440 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    16965 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.664924 oms-mqclient-2.0.0/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-04-21 20:01:30.000000 oms-mqclient-2.0.0/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-04-21 20:01:30.000000 oms-mqclient-2.0.0/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 20:01:30.000000 oms-mqclient-2.0.0/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      286 2023-04-21 20:01:30.000000 oms-mqclient-2.0.0/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-21 20:01:30.000000 oms-mqclient-2.0.0/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.660924 oms-mqclient-2.0.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.664924 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7026 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    20680 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    18702 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8202 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-1.2.0/LICENSE` & `oms-mqclient-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-1.2.0/PKG-INFO` & `oms-mqclient-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 1.2.0
+Version: 2.0.0
 Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
 Project-URL: Source, https://github.com/Observation-Management-Service/MQClient
-Keywords: Observation Management Service,Event Workflow Management Service,python message passing client,message passing,API,mq,apache,pulsar,google,pubsub,gcp,rabbitmq,pika,nats,nats.io,OpenTelemetry,tracing,telemetry,WIPAC,IceCube
+Keywords: Observation Management Service,Event Workflow Management Service,python message passing client,message passing,API,mq,apache,pulsar,pubsub,rabbitmq,pika,nats,nats.io,OpenTelemetry,tracing,telemetry,WIPAC,IceCube
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: pulsar
 Provides-Extra: rabbitmq
-Provides-Extra: gcp
 Provides-Extra: nats
 Provides-Extra: telemetry
 Provides-Extra: dev
 Provides-Extra: integration
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/oms-mqclient)](https://pypi.org/project/oms-mqclient/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Observation-Management-Service/MQClient?include_prereleases)](https://github.com/Observation-Management-Service/MQClient/) [![PyPI - License](https://img.shields.io/pypi/l/oms-mqclient)](https://github.com/Observation-Management-Service/MQClient/blob/master/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/) [![GitHub issues](https://img.shields.io/github/issues/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
 <!--- End of README Badges (automated) --->
 # MQClient
 
-A message-queue client API supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io through a common interface.
+A message-queue client API supporting Apache Pulsar, RabbitMQ, and NATS.io through a common interface.
 
 ### Running with WIPAC Telemetry
 See https://github.com/WIPACrepo/wipac-telemetry-prototype documentation
```

### Comparing `oms-mqclient-1.2.0/README.md` & `oms-mqclient-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/oms-mqclient)](https://pypi.org/project/oms-mqclient/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Observation-Management-Service/MQClient?include_prereleases)](https://github.com/Observation-Management-Service/MQClient/) [![PyPI - License](https://img.shields.io/pypi/l/oms-mqclient)](https://github.com/Observation-Management-Service/MQClient/blob/master/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/) [![GitHub issues](https://img.shields.io/github/issues/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
 <!--- End of README Badges (automated) --->
 # MQClient
 
-A message-queue client API supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io through a common interface.
+A message-queue client API supporting Apache Pulsar, RabbitMQ, and NATS.io through a common interface.
 
 ### Running with WIPAC Telemetry
 See https://github.com/WIPACrepo/wipac-telemetry-prototype documentation
```

### Comparing `oms-mqclient-1.2.0/mqclient/__init__.py` & `oms-mqclient-2.0.0/mqclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.2.0"
+__version__ = "2.0.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-1.2.0/mqclient/broker_client_interface.py` & `oms-mqclient-2.0.0/mqclient/broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-1.2.0/mqclient/broker_client_manager.py` & `oms-mqclient-2.0.0/mqclient/broker_client_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """Manage the different broker_clients."""
 
+from types import ModuleType
+from typing import Dict, Optional
+
 from .broker_client_interface import BrokerClient
 
 # Import all the broker clients at package import, so any bindings can be built/compiled
 # fmt: off
-_INSTALLED_BROKERS = {}
+_INSTALLED_BROKERS: Dict[str, Optional[ModuleType]] = {}
 # Pulsar
 try:
     from .broker_clients import apachepulsar
     _INSTALLED_BROKERS["pulsar"] = apachepulsar
 except (ModuleNotFoundError, ImportError):
     _INSTALLED_BROKERS["pulsar"] = None
-# GCP
-try:
-    from .broker_clients import gcp
-    _INSTALLED_BROKERS["gcp"] = gcp
-except (ModuleNotFoundError, ImportError):
-    _INSTALLED_BROKERS["gcp"] = None
 # NATS
 try:
     from .broker_clients import nats
     _INSTALLED_BROKERS["nats"] = nats
 except (ModuleNotFoundError, ImportError):
     _INSTALLED_BROKERS["nats"] = None
 # RabbitMQ
@@ -31,15 +28,17 @@
     _INSTALLED_BROKERS["rabbitmq"] = None
 # fmt: on
 
 
 def get_broker_client(broker_client_name: str) -> BrokerClient:
     """Get the `BrokerClient` instance per the given name."""
     try:
-        return _INSTALLED_BROKERS[broker_client_name].BrokerClient()
+        module = _INSTALLED_BROKERS[broker_client_name]
     except KeyError:
         raise RuntimeError(f"Unknown broker client: {broker_client_name}")
-    except AttributeError:
+
+    if not module:
         raise RuntimeError(
-            f"Install 'mqclient[{broker_client_name.lower()}]' "
+            f"Install the '{broker_client_name.lower()}' extra "
             f"if you want to use the '{broker_client_name}' broker client"
         )
+    return module.BrokerClient()  # type: ignore[no-any-return]
```

### Comparing `oms-mqclient-1.2.0/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.0.0/mqclient/broker_clients/apachepulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-1.2.0/mqclient/broker_clients/gcp.py` & `oms-mqclient-2.0.0/mqclient/broker_clients/nats.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,336 +1,316 @@
-"""Back-end using GCP."""
+"""Back-end using NATS."""
+
 
 import logging
-import os
-from typing import AsyncGenerator, Generator, List, Optional, Tuple
+import math
+import time
+from functools import partial
+from typing import (
+    Any,
+    AsyncGenerator,
+    Awaitable,
+    Callable,
+    List,
+    Optional,
+    TypeVar,
+    cast,
+)
 
-from google.api_core import exceptions, retry
-from google.cloud import pubsub  # type: ignore[import]
+import nats
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
     RETRY_DELAY,
     TIMEOUT_MILLIS_DEFAULT,
     TRY_ATTEMPTS,
     ClosingFailedException,
     Message,
     Pub,
     RawQueue,
     Sub,
 )
 
-LOGGER = logging.getLogger("mqclient.gcp")
+LOGGER = logging.getLogger("mqclient.nats")
+
+T = TypeVar("T")  # the callable/awaitable return type
+
 
-_DEFAULT_RETRY = retry.Retry(
-    initial=RETRY_DELAY,
-    # maximum=RETRY_DELAY,  # same as initial, not really needed if multiplier=1.0
-    multiplier=1.0,  # change if we want exponential retries
-    deadline=RETRY_DELAY * (TRY_ATTEMPTS - 1),
-)  # Ex: RETRY_DELAY=1, TRY_ATTEMPTS=3: <try> ...1sec... <try> ...1sec... <try>
+async def _anext(gen: AsyncGenerator[Any, Any], default: Any) -> Any:
+    """Provide the functionality of python 3.10's `anext()`.
+
+    https://docs.python.org/3/library/functions.html#anext
+    """
+    try:
+        return await gen.__anext__()
+    except StopAsyncIteration:
+        return default
 
 
-class GCP(RawQueue):
-    """Base GCP wrapper.
+async def try_call(self: "NATS", func: Callable[..., Awaitable[T]]) -> T:
+    """Call `func` with auto-retries."""
+    i = 0
+    while True:
+        if i > 0:
+            LOGGER.debug(
+                f"{log_msgs.TRYCALL_CONNECTION_ERROR_TRY_AGAIN} (attempt #{i+1})..."
+            )
+
+        try:
+            return await func()
+        except nats.errors.TimeoutError:
+            raise
+        except Exception as e:  # pylint:disable=broad-except
+            LOGGER.debug(f"[try_call()] Encountered exception: '{e}'")
+            if i == TRY_ATTEMPTS - 1:
+                LOGGER.debug(log_msgs.TRYCALL_CONNECTION_ERROR_MAX_RETRIES)
+                raise
+
+        await self.close()
+        time.sleep(RETRY_DELAY)
+        await self.connect()
+        i += 1
+
+
+class NATS(RawQueue):
+    """Base NATS wrapper, using JetStream.
 
     Extends:
         RawQueue
     """
 
-    def __init__(self, endpoint: str, project_id: str, topic_id: str) -> None:
+    def __init__(self, endpoint: str, stream_id: str, subject: str) -> None:
         super().__init__()
         LOGGER.info(
-            f"Requested MQClient for project_id/topic_id '{project_id}/{topic_id}' @ {endpoint}"
+            f"Requested MQClient for stream_id/subject '{stream_id}/{subject}' @ {endpoint}"
         )
 
         self.endpoint = endpoint
-        self._project_id = project_id
+        self.subject = subject
+        self.stream_id = stream_id
 
-        # create a temporary PublisherClient just to get `topic_path`
-        self._topic_path = (
-            pubsub.PublisherClient().topic_path(  # pylint: disable=no-member
-                self._project_id, topic_id
-            )
-        )
-        LOGGER.debug(f"Topic Path: {self._topic_path}")
+        self._nats_client: Optional[nats.aio.client.Client] = None
+        self.js: Optional[nats.js.JetStreamContext] = None
+
+        LOGGER.debug(f"Stream & Subject: {stream_id}/{self.subject}")
 
     async def connect(self) -> None:
         """Set up connection and channel."""
         await super().connect()
+        self._nats_client = await nats.connect(self.endpoint)
+        # Create JetStream context
+        self.js = self._nats_client.jetstream(timeout=TIMEOUT_MILLIS_DEFAULT // 1000)
+        await self.js.add_stream(name=self.stream_id, subjects=[self.subject])
 
     async def close(self) -> None:
         """Close connection."""
         await super().close()
-
-    @staticmethod
-    def _create_and_connect_sub(
-        endpoint: str, project_id: str, topic_path: str, subscription_id: str
-    ) -> Tuple[pubsub.SubscriberClient, str]:
-        """Create a subscription, then return a subscriber instance and path.
-
-        If the subscription already exists, the subscription is
-        unaffected.
-        """
-        sub = pubsub.SubscriberClient(client_options={"api_endpoint": endpoint})
-        subscription_path = sub.subscription_path(  # pylint: disable=no-member
-            project_id, subscription_id
-        )
-
-        try:
-            sub.create_subscription(  # pylint: disable=no-member
-                request={
-                    "name": subscription_path,
-                    "topic": topic_path,
-                    "ack_deadline_seconds": 600,  # 10min is the GCP max
-                },
-                retry=_DEFAULT_RETRY,
-            )
-            LOGGER.debug(f"Subscription created ({subscription_path})")
-        except exceptions.AlreadyExists:
-            LOGGER.debug(f"Subscription already exists ({subscription_path})")
-
-        return sub, subscription_path
+        if not self._nats_client:
+            raise ClosingFailedException("No connection to close.")
+        await self._nats_client.close()
 
 
-class GCPPub(GCP, Pub):
-    """Wrapper around PublisherClient, with topic and subscription creation.
+class NATSPub(NATS, Pub):
+    """Wrapper around PublisherClient, using JetStream.
 
     Extends:
-        GCP
+        NATS
         Pub
     """
 
-    def __init__(
-        self,
-        endpoint: str,
-        project_id: str,
-        topic_id: str,
-        subscription_ids: Optional[List[str]] = None,
-    ):
-        LOGGER.debug(
-            f"{log_msgs.INIT_PUB} "
-            f"({endpoint}; {project_id}; {topic_id}; {subscription_ids})"
-        )
-        super().__init__(endpoint, project_id, topic_id)
-        self.pub: Optional[pubsub.PublisherClient] = None
-        self.subscription_ids = subscription_ids if subscription_ids else []
+    def __init__(self, endpoint: str, stream_id: str, subject: str):
+        LOGGER.debug(f"{log_msgs.INIT_PUB} ({endpoint}; {stream_id}; {subject})")
+        super().__init__(endpoint, stream_id, subject)
+        # NATS is pub-centric, so no extra instance needed
 
     async def connect(self) -> None:
         """Set up pub, then create topic and any subscriptions indicated."""
         LOGGER.debug(log_msgs.CONNECTING_PUB)
         await super().connect()
-
-        self.pub = pubsub.PublisherClient(
-            publisher_options=pubsub.types.PublisherOptions(
-                enable_message_ordering=True
-            ),
-            client_options={"api_endpoint": self.endpoint},
-        )
-
-        try:
-            self.pub.create_topic(  # pylint: disable=no-member
-                request={"name": self._topic_path}, retry=_DEFAULT_RETRY
-            )
-            LOGGER.debug(f"Topic created ({self._topic_path})")
-        except exceptions.AlreadyExists:
-            LOGGER.debug(f"Topic already exists ({self._topic_path})")
-        finally:
-            LOGGER.debug(log_msgs.CONNECTED_PUB)
-
-        # Create Any Subscriptions
-        # NOTE - A message published before a given subscription was created will
-        #  usually not be delivered for that subscription. Thus, a message published
-        #  to a topic that has no subscription will not be delivered to any subscriber.
-        for sub_id in self.subscription_ids:
-            GCP._create_and_connect_sub(
-                self.endpoint, self._project_id, self._topic_path, sub_id
-            )
+        LOGGER.debug(log_msgs.CONNECTED_PUB)
 
     async def close(self) -> None:
         """Close pub (no-op)."""
         LOGGER.debug(log_msgs.CLOSING_PUB)
         await super().close()
-        if not self.pub:
-            raise ClosingFailedException("No pub to sub.")
         LOGGER.debug(log_msgs.CLOSED_PUB)
 
     async def send_message(self, msg: bytes) -> None:
         """Send a message (publish)."""
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
-        if not self.pub:
-            raise RuntimeError("publisher is not connected")
+        if not self.js:
+            raise RuntimeError("JetStream is not connected")
 
-        future = self.pub.publish(self._topic_path, msg, retry=_DEFAULT_RETRY)
-        LOGGER.debug(f"Sent Message w/ Origin ID: {future.result()}")
+        ack: nats.js.api.PubAck = await try_call(
+            self, partial(self.js.publish, self.subject, msg)
+        )
+        LOGGER.debug(f"Sent Message w/ Ack: {ack}")
         LOGGER.debug(log_msgs.SENT_MESSAGE)
 
 
-class GCPSub(GCP, Sub):
-    """Wrapper around queue with prefetch-queue QoS.
+class NATSSub(NATS, Sub):
+    """Wrapper around queue with prefetch-queue, using JetStream.
 
     Extends:
-        GCP
+        NATS
         Sub
     """
 
-    def __init__(
-        self, endpoint: str, project_id: str, topic_id: str, subscription_id: str
-    ):
-        LOGGER.debug(
-            f"{log_msgs.INIT_SUB} "
-            f"({endpoint}; {project_id}; {topic_id}; {subscription_id})"
-        )
-        super().__init__(endpoint, project_id, topic_id)
-        self.sub: Optional[pubsub.SubscriberClient] = None
+    def __init__(self, endpoint: str, stream_id: str, subject: str):
+        LOGGER.debug(f"{log_msgs.INIT_SUB} ({endpoint}; {stream_id}; {subject})")
+        super().__init__(endpoint, stream_id, subject)
+        self._subscription: Optional[nats.js.JetStreamContext.PullSubscription] = None
         self.prefetch = 1
 
-        self._subscription_path: Optional[str] = None
-        self._subscription_id = subscription_id
-
     async def connect(self) -> None:
-        """Set up sub (subscriber) and create subscription if necessary.
-
-        NOTE: Based on `examples/gcp/subscriber.create_subscription()`
-        """
+        """Set up sub (pull subscription)."""
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
+        if not self.js:
+            raise RuntimeError("JetStream is not connected.")
 
-        self.sub, self._subscription_path = GCP._create_and_connect_sub(
-            self.endpoint, self._project_id, self._topic_path, self._subscription_id
-        )
+        self._subscription = await self.js.pull_subscribe(self.subject, "psub")
         LOGGER.debug(log_msgs.CONNECTED_SUB)
 
     async def close(self) -> None:
         """Close sub."""
         LOGGER.debug(log_msgs.CLOSING_SUB)
+        if not self._subscription:
+            raise ClosingFailedException("No sub to close.")
         await super().close()
-        if not self.sub:
-            raise ClosingFailedException("No consumer to sub.")
-        try:
-            self.sub.close()
-        except Exception as e:
-            raise ClosingFailedException(str(e)) from e
         LOGGER.debug(log_msgs.CLOSED_SUB)
 
     @staticmethod
     def _to_message(  # type: ignore[override]  # noqa: F821 # pylint: disable=W0221
-        msg: pubsub.types.ReceivedMessage,  # pylint: disable=no-member
+        msg: nats.aio.msg.Msg,  # pylint: disable=no-member
     ) -> Optional[Message]:
-        """Transform GCP-Message to Message type."""
-        return Message(msg.ack_id, msg.message.data)
+        """Transform NATS-Message to Message type."""
+        return Message(msg.reply, msg.data)
+
+    def _from_message(self, msg: Message) -> nats.aio.msg.Msg:
+        """Transform Message instance to NATS-Message.
 
-    def _get_messages(
+        Assumes the message came from this NATSSub instance.
+        """
+        if not self._nats_client:
+            raise RuntimeError("Client is not connected")
+
+        return nats.aio.msg.Msg(
+            _client=self._nats_client,
+            subject=self.subject,
+            reply=cast(str, msg.msg_id),  # we know this is str b/c `_to_message()`
+            data=msg.data,
+            headers=None,  # default
+        )
+
+    async def _get_messages(
         self, timeout_millis: Optional[int], num_messages: int
     ) -> List[Message]:
         """Get n messages.
 
         The subscriber pulls a specific number of messages. The actual
         number of messages pulled may be smaller than `num_messages`.
         """
-        if not self.sub:
-            raise RuntimeError("subscriber is not connected")
+        if not self._subscription:
+            raise RuntimeError("Subscriber is not connected")
 
-        response = self.sub.pull(  # pylint: disable=no-member
-            request={
-                "subscription": self._subscription_path,
-                "max_messages": num_messages,
-            },
-            retry=_DEFAULT_RETRY,
-            # return_immediately=True, # NOTE - use is discourage for performance reasons
-            timeout=timeout_millis / 1000 if timeout_millis else 0,
-            # NOTE - if `retry` is specified, the timeout applies to each individual attempt
-        )
+        if not timeout_millis:
+            timeout_millis = TIMEOUT_MILLIS_DEFAULT
+
+        try:
+            nats_msgs: List[nats.aio.msg.Msg] = await try_call(
+                self,
+                partial(
+                    self._subscription.fetch,
+                    num_messages,
+                    int(math.ceil(timeout_millis / 1000)),
+                ),
+            )
+        except nats.errors.TimeoutError:
+            return []
 
         msgs = []
-        for recvd in response.received_messages:
-            LOGGER.debug(f"Got Message w/ Origin ID: {recvd.message.message_id}")
-            msg = GCPSub._to_message(recvd)
+        for recvd in nats_msgs:
+            msg = self._to_message(recvd)
             if msg:
                 msgs.append(msg)
         return msgs
 
     async def get_message(
         self, timeout_millis: Optional[int] = TIMEOUT_MILLIS_DEFAULT
     ) -> Optional[Message]:
-        """Get a message.
-
-        NOTE: Based on `examples/gcp/subscriber.synchronous_pull()`
-        """
+        """Get a message."""
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
+        if not self._subscription:
+            raise RuntimeError("Subscriber is not connected.")
 
         try:
-            msg = self._get_messages(timeout_millis, 1)[0]
-            LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg.msg_id!r}).")
+            msg = (await self._get_messages(timeout_millis, 1))[0]
+            LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg}).")
             return msg
-        except IndexError:  # NOTE - on timeout -> this will be len=0
+        except IndexError:
             LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
             return None
 
-    def _gen_messages(
+    async def _gen_messages(
         self, timeout_millis: Optional[int], num_messages: int
-    ) -> Generator[Message, None, None]:
+    ) -> AsyncGenerator[Message, None]:
         """Continuously generate messages until there are no more."""
+        if not self._subscription:
+            raise RuntimeError("Subscriber is not connected.")
+
         while True:
-            msgs = self._get_messages(timeout_millis, num_messages)
+            msgs = await self._get_messages(timeout_millis, num_messages)
             if not msgs:
                 return
             for msg in msgs:
                 yield msg
 
     async def ack_message(self, msg: Message) -> None:
         """Ack a message from the queue."""
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
-        if not self.sub:
+        if not self._subscription:
             raise RuntimeError("subscriber is not connected")
 
         # Acknowledges the received messages so they will not be sent again.
-        self.sub.acknowledge(  # pylint: disable=no-member
-            request={"subscription": self._subscription_path, "ack_ids": [msg.msg_id]}
-        )
+        await try_call(self, partial(self._from_message(msg).ack))
         LOGGER.debug(f"{log_msgs.ACKED_MESSAGE} ({msg.msg_id!r}).")
 
     async def reject_message(self, msg: Message) -> None:
         """Reject (nack) a message from the queue."""
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
-        if not self.sub:
+        if not self._subscription:
             raise RuntimeError("subscriber is not connected")
 
-        # override the subscription-level ack deadline to fast-track redelivery
-        self.sub.modify_ack_deadline(  # pylint: disable=no-member
-            request={
-                "subscription": self._subscription_path,
-                "ack_ids": [msg.msg_id],
-                "ack_deadline_seconds": 0,
-            }
-        )
+        await try_call(self, partial(self._from_message(msg).nak))  # yes, it's "nak"
         LOGGER.debug(f"{log_msgs.NACKED_MESSAGE} ({msg.msg_id!r}).")
 
-    async def message_generator(  # type: ignore[override] # there's a mypy bug here
+    async def message_generator(
         self, timeout: int = 60, propagate_error: bool = True
     ) -> AsyncGenerator[Optional[Message], None]:
         """Yield Messages.
 
         Generate messages with variable timeout.
         Yield `None` on `throw()`.
 
         Keyword Arguments:
             timeout {int} -- timeout in seconds for inactivity (default: {60})
             propagate_error {bool} -- should errors from downstream code kill the generator? (default: {True})
         """
         LOGGER.debug(log_msgs.MSGGEN_ENTERED)
-        if not self.sub:
+        if not self._subscription:
             raise RuntimeError("subscriber is not connected")
 
         msg = None
         try:
             gen = self._gen_messages(timeout * 1000, self.prefetch)
             while True:
                 # get message
                 LOGGER.debug(log_msgs.MSGGEN_GET_NEW_MESSAGE)
-                msg = next(gen, None)
+                msg = await _anext(gen, None)
                 if msg is None:
                     LOGGER.info(log_msgs.MSGGEN_NO_MESSAGE_LOOK_BACK_IN_QUEUE)
                     break
 
                 # yield message to consumer
                 try:
                     LOGGER.debug(f"{log_msgs.MSGGEN_YIELDING_MESSAGE} [{msg}]")
@@ -353,80 +333,54 @@
         # garbage collection (or explicit generator close(), or break in consumer's loop)
         except GeneratorExit:
             LOGGER.debug(log_msgs.MSGGEN_GENERATOR_EXITING)
             LOGGER.debug(log_msgs.MSGGEN_GENERATOR_EXITED)
 
 
 class BrokerClient(broker_client_interface.BrokerClient):
-    """GCP Pub-Sub BrokerClient Factory.
+    """NATS Pub-Sub BrokerClient Factory.
 
     Extends:
         BrokerClient
     """
 
-    NAME = "gcp"
-
-    # NOTE - this could be an enviro var, but it is always constant across all members
-    PROJECT_ID = "i3-gcp-proj"
-
-    # NOTE - use single shared subscription
-    # (making multiple unique subscription ids would create independent subscriptions)
-    # See https://thecloudgirl.dev/images/pubsub.jpg
-    SUBSCRIPTION_ID = "i3-gcp-sub"
-
-    # NOTE - this is an environment variable, which should override the host address
-    PUBSUB_EMULATOR_HOST = "PUBSUB_EMULATOR_HOST"
-
-    @staticmethod
-    def _figure_host_address(address: str) -> str:
-        """If the pub-sub emulator enviro var is set, use that address."""
-        try:
-            emulator = os.environ[BrokerClient.PUBSUB_EMULATOR_HOST]
-            LOGGER.warning(
-                f"Environment variable `{BrokerClient.PUBSUB_EMULATOR_HOST}` is set: "
-                f"using Pub-Sub Emulator at {emulator} (overriding `{address}`)."
-            )
-            return emulator
-        except KeyError:
-            return address
+    NAME = "nats"
 
     @staticmethod
     async def create_pub_queue(
         address: str,
         name: str,
         auth_token: str,
         ack_timeout: Optional[int],
-    ) -> GCPPub:
+    ) -> NATSPub:
         """Create a publishing queue.
 
         # NOTE - `auth_token` is not used currently
         """
-        q = GCPPub(  # pylint: disable=invalid-name
-            BrokerClient._figure_host_address(address),
-            BrokerClient.PROJECT_ID,
-            name,
-            [f"{BrokerClient.SUBSCRIPTION_ID}-{name}"],
+        q = NATSPub(  # pylint: disable=invalid-name
+            address,
+            name + "-stream",
+            name + "-subject",
         )
         await q.connect()
         return q
 
     @staticmethod
     async def create_sub_queue(
         address: str,
         name: str,
         prefetch: int,
         auth_token: str,
         ack_timeout: Optional[int],
-    ) -> GCPSub:
+    ) -> NATSSub:
         """Create a subscription queue.
 
         # NOTE - `auth_token` is not used currently
         """
-        q = GCPSub(  # pylint: disable=invalid-name
-            BrokerClient._figure_host_address(address),
-            BrokerClient.PROJECT_ID,
-            name,
-            f"{BrokerClient.SUBSCRIPTION_ID}-{name}",
+        q = NATSSub(  # pylint: disable=invalid-name
+            address,
+            name + "-stream",
+            name + "-subject",
         )
         q.prefetch = prefetch
         await q.connect()
         return q
```

### Comparing `oms-mqclient-1.2.0/mqclient/broker_clients/nats.py` & `oms-mqclient-2.0.0/mqclient/broker_clients/rabbitmq.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,317 +1,336 @@
-"""Back-end using NATS."""
-
+"""Back-end using RabbitMQ."""
 
 import logging
-import math
 import time
+import urllib
 from functools import partial
-from typing import (
-    Any,
-    AsyncGenerator,
-    Awaitable,
-    Callable,
-    List,
-    Optional,
-    TypeVar,
-    cast,
-)
+from typing import Any, AsyncGenerator, Callable, Dict, Optional, Tuple, Union
 
-import nats
+import pika  # type: ignore
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
     RETRY_DELAY,
     TIMEOUT_MILLIS_DEFAULT,
     TRY_ATTEMPTS,
+    AlreadyClosedException,
     ClosingFailedException,
+    ConnectingFailedException,
     Message,
     Pub,
     RawQueue,
     Sub,
 )
 
-LOGGER = logging.getLogger("mqclient.nats")
+StrDict = Dict[str, Any]
 
-T = TypeVar("T")  # the callable/awaitable return type
+LOGGER = logging.getLogger("mqclient.rabbitmq")
 
 
-async def _anext(gen: AsyncGenerator[Any, Any], default: Any) -> Any:
-    """Provide the functionality of python 3.10's `anext()`.
+HUMAN_PATTERN = "[SCHEME://][USER[:PASS]@]HOST[:PORT][/VIRTUAL_HOST]"
 
-    https://docs.python.org/3/library/functions.html#anext
-    """
-    try:
-        return await gen.__anext__()
-    except StopAsyncIteration:
-        return default
 
+def _parse_url(url: str) -> Tuple[StrDict, Optional[str], Optional[str]]:
+    if "://" not in url:
+        url = "//" + url
+    result = urllib.parse.urlparse(url)
 
-async def try_call(self: "NATS", func: Callable[..., Awaitable[T]]) -> T:
-    """Call `func` with auto-retries."""
-    i = 0
-    while True:
-        if i > 0:
-            LOGGER.debug(
-                f"{log_msgs.TRYCALL_CONNECTION_ERROR_TRY_AGAIN} (attempt #{i+1})..."
-            )
+    parts = dict(
+        scheme=result.scheme,
+        host=result.hostname,
+        port=result.port,
+        virtual_host=result.path.lstrip("/"),
+    )
+    # for putting into ConnectionParameters filter ""/None (will rely on defaults)
+    parts = {k: v for k, v in parts.items() if v}  # host=..., etc.
 
-        try:
-            return await func()
-        except nats.errors.TimeoutError:
-            raise
-        except Exception as e:  # pylint:disable=broad-except
-            LOGGER.debug(f"[try_call()] Encountered exception: '{e}'")
-            if i == TRY_ATTEMPTS - 1:
-                LOGGER.debug(log_msgs.TRYCALL_CONNECTION_ERROR_MAX_RETRIES)
-                raise
+    # check validity
+    if not parts or "host" not in parts:
+        raise RuntimeError(f"Invalid address: {url} (format: {HUMAN_PATTERN})")
 
-        await self.close()
-        time.sleep(RETRY_DELAY)
-        await self.connect()
-        i += 1
+    return parts, result.username, result.password
+
+
+def _get_credentials(
+    username: Optional[str], password: Optional[str], auth_token: str
+) -> Optional[pika.credentials.PlainCredentials]:
+    if auth_token:
+        password = auth_token
 
+    # Case 1: username/password
+    if username and password:
+        return pika.credentials.PlainCredentials(username, password)
+    # Case 2: Only password/token -- Ex: keycloak
+    elif (not username) and password:
+        return pika.credentials.PlainCredentials("", password)
+    # Error: no password for user
+    elif username and (not password):
+        raise RuntimeError("username given but no password or token")
+    # Case 3: no auth -- rabbitmq uses guest/guest
+    else:  # not username and not password
+        return None
 
-class NATS(RawQueue):
-    """Base NATS wrapper, using JetStream.
+
+class RabbitMQ(RawQueue):
+    """Base RabbitMQ wrapper.
 
     Extends:
         RawQueue
     """
 
-    def __init__(self, endpoint: str, stream_id: str, subject: str) -> None:
+    def __init__(
+        self,
+        address: str,
+        queue: str,
+        auth_token: str,
+        ack_timeout: Optional[int],
+    ) -> None:
         super().__init__()
-        LOGGER.info(
-            f"Requested MQClient for stream_id/subject '{stream_id}/{subject}' @ {endpoint}"
-        )
-
-        self.endpoint = endpoint
-        self.subject = subject
-        self.stream_id = stream_id
+        LOGGER.info(f"Requested MQClient for queue '{queue}' @ {address}")
+        cp_args, username, password = _parse_url(address)
 
-        self._nats_client: Optional[nats.aio.client.Client] = None
-        self.js: Optional[nats.js.JetStreamContext] = None
-
-        LOGGER.debug(f"Stream & Subject: {stream_id}/{self.subject}")
+        # set up connection parameters
+        if creds := _get_credentials(username, password, auth_token):
+            cp_args["credentials"] = creds
+        if ack_timeout:
+            cp_args["heartbeat"] = ack_timeout
+        self.parameters = pika.connection.ConnectionParameters(**cp_args)
+
+        self.queue = queue
+        self.connection: Optional[pika.BlockingConnection] = None
+        self.channel: Optional[pika.adapters.blocking_connection.BlockingChannel] = None
 
     async def connect(self) -> None:
         """Set up connection and channel."""
         await super().connect()
-        self._nats_client = await nats.connect(self.endpoint)
-        # Create JetStream context
-        self.js = self._nats_client.jetstream(timeout=TIMEOUT_MILLIS_DEFAULT // 1000)
-        await self.js.add_stream(name=self.stream_id, subjects=[self.subject])
+        LOGGER.info(f"Connecting with parameters={self.parameters}")
+        self.connection = pika.BlockingConnection(self.parameters)
+        self.channel = self.connection.channel()
+        """
+        We need to discuss how many RabbitMQ instances we want to run
+        the default is that the quorum queue is spread across 3 nodes
+        so 1 can fail without issue. Maybe we want to up this for
+        more production workloads
+        """
+        self.channel.queue_declare(
+            queue=self.queue, durable=True, arguments={"x-queue-type": "quorum"}
+        )
 
     async def close(self) -> None:
         """Close connection."""
         await super().close()
-        if not self._nats_client:
+
+        if not self.channel:
+            raise ClosingFailedException("No channel to close.")
+        if not self.connection:
             raise ClosingFailedException("No connection to close.")
-        await self._nats_client.close()
+        if self.connection.is_closed:
+            raise AlreadyClosedException()
+
+        try:
+            self.channel.cancel()
+            self.connection.close()
+        except Exception as e:
+            raise ClosingFailedException() from e
+
+        if self.channel.is_open:
+            LOGGER.warning("Channel remains open after connection close.")
 
 
-class NATSPub(NATS, Pub):
-    """Wrapper around PublisherClient, using JetStream.
+class RabbitMQPub(RabbitMQ, Pub):
+    """Wrapper around queue with delivery-confirm mode in the channel.
 
     Extends:
-        NATS
+        RabbitMQ
         Pub
     """
 
-    def __init__(self, endpoint: str, stream_id: str, subject: str):
-        LOGGER.debug(f"{log_msgs.INIT_PUB} ({endpoint}; {stream_id}; {subject})")
-        super().__init__(endpoint, stream_id, subject)
-        # NATS is pub-centric, so no extra instance needed
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        LOGGER.debug(f"{log_msgs.INIT_PUB} ({args}; {kwargs})")
+        super().__init__(*args, **kwargs)
 
     async def connect(self) -> None:
-        """Set up pub, then create topic and any subscriptions indicated."""
+        """Set up connection, channel, and queue.
+
+        Turn on delivery confirmations.
+        """
         LOGGER.debug(log_msgs.CONNECTING_PUB)
         await super().connect()
+
+        if not self.channel:
+            raise ConnectingFailedException("No channel to configure connection.")
+
+        self.channel.confirm_delivery()
+
         LOGGER.debug(log_msgs.CONNECTED_PUB)
 
     async def close(self) -> None:
-        """Close pub (no-op)."""
+        """Close connection."""
         LOGGER.debug(log_msgs.CLOSING_PUB)
         await super().close()
         LOGGER.debug(log_msgs.CLOSED_PUB)
 
     async def send_message(self, msg: bytes) -> None:
-        """Send a message (publish)."""
+        """Send a message on a queue.
+
+        Args:
+            address (str): address of queue
+            name (str): name of queue on address
+
+        Returns:
+            RawQueue: queue
+        """
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
-        if not self.js:
-            raise RuntimeError("JetStream is not connected")
+        if not self.channel:
+            raise RuntimeError("queue is not connected")
 
-        ack: nats.js.api.PubAck = await try_call(
-            self, partial(self.js.publish, self.subject, msg)
+        await try_call(
+            self,
+            partial(
+                self.channel.basic_publish,
+                exchange="",
+                routing_key=self.queue,
+                body=msg,
+            ),
         )
-        LOGGER.debug(f"Sent Message w/ Ack: {ack}")
         LOGGER.debug(log_msgs.SENT_MESSAGE)
 
 
-class NATSSub(NATS, Sub):
-    """Wrapper around queue with prefetch-queue, using JetStream.
+class RabbitMQSub(RabbitMQ, Sub):
+    """Wrapper around queue with prefetch-queue QoS.
 
     Extends:
-        NATS
+        RabbitMQ
         Sub
     """
 
-    def __init__(self, endpoint: str, stream_id: str, subject: str):
-        LOGGER.debug(f"{log_msgs.INIT_SUB} ({endpoint}; {stream_id}; {subject})")
-        super().__init__(endpoint, stream_id, subject)
-        self._subscription: Optional[nats.js.JetStreamContext.PullSubscription] = None
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        LOGGER.debug(f"{log_msgs.INIT_SUB} ({args}; {kwargs})")
+        super().__init__(*args, **kwargs)
+        self.consumer_id = None
         self.prefetch = 1
 
     async def connect(self) -> None:
-        """Set up sub (pull subscription)."""
+        """Set up connection, channel, and queue.
+
+        Turn on prefetching.
+        """
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
-        if not self.js:
-            raise RuntimeError("JetStream is not connected.")
 
-        self._subscription = await self.js.pull_subscribe(self.subject, "psub")
+        if not self.channel:
+            raise ConnectingFailedException("No channel to configure connection.")
+
+        self.channel.basic_qos(prefetch_count=self.prefetch)
+        # global_qos=False b/c using quorum queues
+        # https://www.rabbitmq.com/quorum-queues.html#global-qos
+
         LOGGER.debug(log_msgs.CONNECTED_SUB)
 
     async def close(self) -> None:
-        """Close sub."""
+        """Close connection.
+
+        Also, channel will be canceled (rejects all pending ackable
+        messages).
+        """
         LOGGER.debug(log_msgs.CLOSING_SUB)
-        if not self._subscription:
-            raise ClosingFailedException("No sub to close.")
         await super().close()
         LOGGER.debug(log_msgs.CLOSED_SUB)
 
     @staticmethod
     def _to_message(  # type: ignore[override]  # noqa: F821 # pylint: disable=W0221
-        msg: nats.aio.msg.Msg,  # pylint: disable=no-member
+        method_frame: Optional[pika.spec.Basic.GetOk], body: Optional[Union[str, bytes]]
     ) -> Optional[Message]:
-        """Transform NATS-Message to Message type."""
-        return Message(msg.reply, msg.data)
-
-    def _from_message(self, msg: Message) -> nats.aio.msg.Msg:
-        """Transform Message instance to NATS-Message.
-
-        Assumes the message came from this NATSSub instance.
-        """
-        if not self._nats_client:
-            raise RuntimeError("Client is not connected")
-
-        return nats.aio.msg.Msg(
-            _client=self._nats_client,
-            subject=self.subject,
-            reply=cast(str, msg.msg_id),  # we know this is str b/c `_to_message()`
-            data=msg.data,
-            headers=None,  # default
-        )
-
-    async def _get_messages(
-        self, timeout_millis: Optional[int], num_messages: int
-    ) -> List[Message]:
-        """Get n messages.
-
-        The subscriber pulls a specific number of messages. The actual
-        number of messages pulled may be smaller than `num_messages`.
-        """
-        if not self._subscription:
-            raise RuntimeError("Subscriber is not connected")
-
-        if not timeout_millis:
-            timeout_millis = TIMEOUT_MILLIS_DEFAULT
-
-        try:
-            nats_msgs: List[nats.aio.msg.Msg] = await try_call(
-                self,
-                partial(
-                    self._subscription.fetch,
-                    num_messages,
-                    int(math.ceil(timeout_millis / 1000)),
-                ),
-            )
-        except nats.errors.TimeoutError:
-            return []
+        """Transform RabbitMQ-Message to Message type."""
+        if not method_frame or body is None:
+            return None
 
-        msgs = []
-        for recvd in nats_msgs:
-            msg = self._to_message(recvd)
-            if msg:
-                msgs.append(msg)
-        return msgs
+        if isinstance(body, str):
+            return Message(method_frame.delivery_tag, body.encode())
+        else:
+            return Message(method_frame.delivery_tag, body)
 
     async def get_message(
         self, timeout_millis: Optional[int] = TIMEOUT_MILLIS_DEFAULT
     ) -> Optional[Message]:
-        """Get a message."""
+        """Get a message from a queue."""
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
-        if not self._subscription:
-            raise RuntimeError("Subscriber is not connected.")
+        if not self.channel:
+            raise RuntimeError("queue is not connected")
 
-        try:
-            msg = (await self._get_messages(timeout_millis, 1))[0]
-            LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg}).")
+        gen = partial(
+            self.channel.consume,
+            self.queue,
+            inactivity_timeout=timeout_millis / 1000.0 if timeout_millis else None,
+        )
+        async for method_frame, _, body in try_yield(self, gen):
+            msg = RabbitMQSub._to_message(method_frame, body)  # None -> timeout
+            break  # get just one message
+
+        # self.channel.cancel()  # this is done by `open_sub_one()` *after* ack/nack via `close()`
+
+        if msg:
+            LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg.msg_id!r}).")
             return msg
-        except IndexError:
+        else:
             LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
             return None
 
-    async def _gen_messages(
-        self, timeout_millis: Optional[int], num_messages: int
-    ) -> AsyncGenerator[Message, None]:
-        """Continuously generate messages until there are no more."""
-        if not self._subscription:
-            raise RuntimeError("Subscriber is not connected.")
-
-        while True:
-            msgs = await self._get_messages(timeout_millis, num_messages)
-            if not msgs:
-                return
-            for msg in msgs:
-                yield msg
-
     async def ack_message(self, msg: Message) -> None:
-        """Ack a message from the queue."""
+        """Ack a message from the queue.
+
+        Note that RabbitMQ acks messages in-order, so acking message 3
+        of 3 in-progress messages will ack them all.
+        """
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
-        if not self._subscription:
-            raise RuntimeError("subscriber is not connected")
+        if not self.channel:
+            raise RuntimeError("queue is not connected")
 
-        # Acknowledges the received messages so they will not be sent again.
-        await try_call(self, partial(self._from_message(msg).ack))
+        await try_call(self, partial(self.channel.basic_ack, msg.msg_id))
         LOGGER.debug(f"{log_msgs.ACKED_MESSAGE} ({msg.msg_id!r}).")
 
     async def reject_message(self, msg: Message) -> None:
-        """Reject (nack) a message from the queue."""
+        """Reject (nack) a message from the queue.
+
+        Note that RabbitMQ acks messages in-order, so nacking message 3
+        of 3 in-progress messages will nack them all.
+        """
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
-        if not self._subscription:
-            raise RuntimeError("subscriber is not connected")
+        if not self.channel:
+            raise RuntimeError("queue is not connected")
 
-        await try_call(self, partial(self._from_message(msg).nak))  # yes, it's "nak"
+        await try_call(self, partial(self.channel.basic_nack, msg.msg_id))
         LOGGER.debug(f"{log_msgs.NACKED_MESSAGE} ({msg.msg_id!r}).")
 
     async def message_generator(
         self, timeout: int = 60, propagate_error: bool = True
     ) -> AsyncGenerator[Optional[Message], None]:
         """Yield Messages.
 
         Generate messages with variable timeout.
         Yield `None` on `throw()`.
 
         Keyword Arguments:
             timeout {int} -- timeout in seconds for inactivity (default: {60})
-            propagate_error {bool} -- should errors from downstream code kill the generator? (default: {True})
+            propagate_error -- should errors from downstream kill the generator? (default: {True})
         """
         LOGGER.debug(log_msgs.MSGGEN_ENTERED)
-        if not self._subscription:
-            raise RuntimeError("subscriber is not connected")
+        if not self.channel:
+            raise RuntimeError("queue is not connected")
 
         msg = None
         try:
-            gen = self._gen_messages(timeout * 1000, self.prefetch)
-            while True:
+            gen = partial(self.channel.consume, self.queue, inactivity_timeout=timeout)
+
+            async for method_frame, _, body in try_yield(self, gen):
                 # get message
+                msg = RabbitMQSub._to_message(method_frame, body)
                 LOGGER.debug(log_msgs.MSGGEN_GET_NEW_MESSAGE)
-                msg = await _anext(gen, None)
-                if msg is None:
+                if not msg:
                     LOGGER.info(log_msgs.MSGGEN_NO_MESSAGE_LOOK_BACK_IN_QUEUE)
                     break
 
                 # yield message to consumer
                 try:
                     LOGGER.debug(f"{log_msgs.MSGGEN_YIELDING_MESSAGE} [{msg}]")
                     yield msg
@@ -326,61 +345,134 @@
                         exc_info=True,
                     )
                     yield None  # hand back to consumer
                 # consumer requests again, aka next()
                 else:
                     pass
 
-        # garbage collection (or explicit generator close(), or break in consumer's loop)
+        # Garbage Collection (or explicit generator close(), or break in consumer's loop)
         except GeneratorExit:
             LOGGER.debug(log_msgs.MSGGEN_GENERATOR_EXITING)
             LOGGER.debug(log_msgs.MSGGEN_GENERATOR_EXITED)
 
+        # Done with generator, one way or another
+        finally:
+            self.channel.cancel()
+
+
+async def try_call(queue: RabbitMQ, func: Callable[..., Any]) -> Any:
+    """Try to call `func` and return value.
+
+    Try up to `TRY_ATTEMPTS` times, for connection-related errors.
+    """
+    for i in range(TRY_ATTEMPTS):
+        if i > 0:
+            LOGGER.debug(
+                f"{log_msgs.TRYCALL_CONNECTION_ERROR_TRY_AGAIN} (attempt #{i+1})..."
+            )
+
+        try:
+            return func()
+        except pika.exceptions.ConnectionClosedByBroker:
+            LOGGER.debug(log_msgs.TRYCALL_CONNECTION_CLOSED_BY_BROKER)
+        # Do not recover on channel errors
+        except pika.exceptions.AMQPChannelError as err:
+            LOGGER.error(f"{log_msgs.TRYCALL_RAISE_AMQP_CHANNEL_ERROR} {err}.")
+            raise
+        # Recover on all other connection errors
+        except pika.exceptions.AMQPConnectionError:
+            LOGGER.debug(log_msgs.TRYCALL_AMQP_CONNECTION_ERROR)
+
+        await queue.close()
+        time.sleep(RETRY_DELAY)
+        await queue.connect()
+
+    LOGGER.debug(log_msgs.TRYCALL_CONNECTION_ERROR_MAX_RETRIES)
+    raise Exception("RabbitMQ connection error")
+
+
+async def try_yield(
+    queue: RabbitMQ, func: Callable[..., Any]
+) -> AsyncGenerator[Any, None]:
+    """Try to call `func` and yield value(s).
+
+    Try up to `TRY_ATTEMPTS` times, for connection-related errors.
+    """
+    for i in range(TRY_ATTEMPTS):
+        if i > 0:
+            LOGGER.debug(
+                f"{log_msgs.TRYYIELD_CONNECTION_ERROR_TRY_AGAIN} (attempt #{i+1})..."
+            )
+
+        try:
+            for x in func():  # pylint: disable=invalid-name
+                yield x
+        except pika.exceptions.ConnectionClosedByBroker:
+            LOGGER.debug(log_msgs.TRYYIELD_CONNECTION_CLOSED_BY_BROKER)
+        # Do not recover on channel errors
+        except pika.exceptions.AMQPChannelError as err:
+            LOGGER.error(f"{log_msgs.TRYYIELD_RAISE_AMQP_CHANNEL_ERROR} {err}.")
+            raise
+        # Recover on all other connection errors
+        except pika.exceptions.AMQPConnectionError:
+            LOGGER.debug(log_msgs.TRYYIELD_AMQP_CONNECTION_ERROR)
+
+        await queue.close()
+        time.sleep(RETRY_DELAY)
+        await queue.connect()
+
+    LOGGER.debug(log_msgs.TRYYIELD_CONNECTION_ERROR_MAX_RETRIES)
+    raise Exception("RabbitMQ connection error")
+
 
 class BrokerClient(broker_client_interface.BrokerClient):
-    """NATS Pub-Sub BrokerClient Factory.
+    """RabbitMQ Pub-Sub BrokerClient Factory.
 
     Extends:
         BrokerClient
     """
 
-    NAME = "nats"
+    NAME = "rabbitmq"
 
     @staticmethod
     async def create_pub_queue(
         address: str,
         name: str,
         auth_token: str,
         ack_timeout: Optional[int],
-    ) -> NATSPub:
+    ) -> RabbitMQPub:
         """Create a publishing queue.
 
-        # NOTE - `auth_token` is not used currently
+        Args:
+            address (str): address of queue
+            name (str): name of queue on address
+
+        Returns:
+            RawQueue: queue
         """
-        q = NATSPub(  # pylint: disable=invalid-name
-            address,
-            name + "-stream",
-            name + "-subject",
-        )
+        # pylint: disable=invalid-name
+        q = RabbitMQPub(address, name, auth_token, ack_timeout)
         await q.connect()
         return q
 
     @staticmethod
     async def create_sub_queue(
         address: str,
         name: str,
         prefetch: int,
         auth_token: str,
         ack_timeout: Optional[int],
-    ) -> NATSSub:
+    ) -> RabbitMQSub:
         """Create a subscription queue.
 
-        # NOTE - `auth_token` is not used currently
+        Args:
+            address (str): address of queue
+            name (str): name of queue on address
+
+        Returns:
+            RawQueue: queue
         """
-        q = NATSSub(  # pylint: disable=invalid-name
-            address,
-            name + "-stream",
-            name + "-subject",
-        )
+        # pylint: disable=invalid-name
+        q = RabbitMQSub(address, name, auth_token, ack_timeout)
         q.prefetch = prefetch
         await q.connect()
         return q
```

### Comparing `oms-mqclient-1.2.0/mqclient/log_msgs.py` & `oms-mqclient-2.0.0/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-1.2.0/mqclient/queue.py` & `oms-mqclient-2.0.0/mqclient/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,17 +209,14 @@
         instance is not.
 
         Example:
             async with queue.open_sub() as stream:
                 async for msg in stream:
                     print(msg)
 
-        NOTE: If using the GCP broker_client, a message is allocated for
-        redelivery if the consumer's iteration takes longer than 10 minutes.
-
         Returns:
             QueueSubResource -- context manager and generator object
         """
         LOGGER.debug("Creating new QueueSubResource instance.")
         return QueueSubResource(self)
 
     @contextlib.asynccontextmanager  # needs to wrap @wtt stuff to span children correctly
@@ -236,17 +233,14 @@
         """Open a context to receive a single messages from the queue.
 
         This is an async context manager. If an exception is raised
         (inside the context), the message is rejected, the context is
         exited, and exception can be re-raised if configured by
         `except_errors`.
 
-        NOTE: If using the GCP broker_client, a message is allocated for
-        redelivery if the context is open for longer than 10 minutes.
-
         Example:
             async with q.open_sub_one() as msg:
                 print(msg)
 
         Decorators:
             contextlib.asynccontextmanager
 
@@ -459,15 +453,15 @@
             await self.queue._safe_ack(self._sub, self.msg)
 
         @wtt.spanned(
             kind=wtt.SpanKind.CONSUMER,
             carrier="msg.headers",
             carrier_relation=wtt.CarrierRelation.LINK,
         )
-        def get_message_callback(msg: Message) -> Message:
+        def get_message_callback(msg: Optional[Message]) -> Optional[Message]:
             return msg
 
         try:
             self.msg = get_message_callback(await self._gen.__anext__())
         except StopAsyncIteration:
             self.msg = None  # signal there is no message to ack/nack in `__aexit__()`
             LOGGER.debug(
@@ -490,9 +484,13 @@
             "self.queue._name",
             "self.queue._prefetch",
             "self.queue.timeout",
         ],
     )
     async def nack_current(self) -> None:
         """Manually nack the current (most recently yielded) message."""
+        if not (self._sub and self._gen):
+            raise RuntimeError(self.RUNTIME_ERROR_CONTEXT_STRING)
+        if not self.msg:  # case: calling after iterator stopped (unusual but possible)
+            return
         # pylint:disable=protected-access
         await self.queue._safe_nack(self._sub, self.msg)
```

### Comparing `oms-mqclient-1.2.0/mqclient/telemetry.py` & `oms-mqclient-2.0.0/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-1.2.0/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.0.0/oms_mqclient.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 1.2.0
+Version: 2.0.0
 Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
 Project-URL: Source, https://github.com/Observation-Management-Service/MQClient
-Keywords: Observation Management Service,Event Workflow Management Service,python message passing client,message passing,API,mq,apache,pulsar,google,pubsub,gcp,rabbitmq,pika,nats,nats.io,OpenTelemetry,tracing,telemetry,WIPAC,IceCube
+Keywords: Observation Management Service,Event Workflow Management Service,python message passing client,message passing,API,mq,apache,pulsar,pubsub,rabbitmq,pika,nats,nats.io,OpenTelemetry,tracing,telemetry,WIPAC,IceCube
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: pulsar
 Provides-Extra: rabbitmq
-Provides-Extra: gcp
 Provides-Extra: nats
 Provides-Extra: telemetry
 Provides-Extra: dev
 Provides-Extra: integration
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
 [![PyPI](https://img.shields.io/pypi/v/oms-mqclient)](https://pypi.org/project/oms-mqclient/) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Observation-Management-Service/MQClient?include_prereleases)](https://github.com/Observation-Management-Service/MQClient/) [![PyPI - License](https://img.shields.io/pypi/l/oms-mqclient)](https://github.com/Observation-Management-Service/MQClient/blob/master/LICENSE) [![Lines of code](https://img.shields.io/tokei/lines/github/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/) [![GitHub issues](https://img.shields.io/github/issues/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aopen) [![GitHub pull requests](https://img.shields.io/github/issues-pr/Observation-Management-Service/MQClient)](https://github.com/Observation-Management-Service/MQClient/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Aopen) 
 <!--- End of README Badges (automated) --->
 # MQClient
 
-A message-queue client API supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io through a common interface.
+A message-queue client API supporting Apache Pulsar, RabbitMQ, and NATS.io through a common interface.
 
 ### Running with WIPAC Telemetry
 See https://github.com/WIPACrepo/wipac-telemetry-prototype documentation
```

### Comparing `oms-mqclient-1.2.0/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.0.0/oms_mqclient.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,28 @@
 mqclient/config.py
 mqclient/log_msgs.py
 mqclient/py.typed
 mqclient/queue.py
 mqclient/telemetry.py
 mqclient/broker_clients/__init__.py
 mqclient/broker_clients/apachepulsar.py
-mqclient/broker_clients/gcp.py
 mqclient/broker_clients/nats.py
 mqclient/broker_clients/rabbitmq.py
 oms_mqclient.egg-info/PKG-INFO
 oms_mqclient.egg-info/SOURCES.txt
 oms_mqclient.egg-info/dependency_links.txt
 oms_mqclient.egg-info/requires.txt
 oms_mqclient.egg-info/top_level.txt
 tests/abstract_broker_client_tests/__init__.py
 tests/abstract_broker_client_tests/integrate_broker_client_interface.py
 tests/abstract_broker_client_tests/integrate_queue.py
 tests/abstract_broker_client_tests/unit_tests.py
 tests/abstract_broker_client_tests/utils.py
 tests/integrate/__init__.py
 tests/integrate/conftest.py
-tests/integrate/test_gcp.py
 tests/integrate/test_nats.py
 tests/integrate/test_pulsar.py
 tests/integrate/test_rabbitmq.py
 tests/unit/__init__.py
 tests/unit/pulsar/__init__.py
 tests/unit/pulsar/test_pulsar.py
 tests/unit/rabbitmq/__init__.py
```

### Comparing `oms-mqclient-1.2.0/setup.cfg` & `oms-mqclient-2.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [wipac:cicd_setup_builder]
 pypi_name = oms-mqclient
 python_min = 3.8
 author = WIPAC Developers
 author_email = developers@icecube.wisc.edu
-keywords_spaced = "Observation Management Service" "Event Workflow Management Service" "python message passing client" "message passing" API mq apache pulsar google pubsub gcp rabbitmq pika nats nats.io OpenTelemetry tracing telemetry
+keywords_spaced = "Observation Management Service" "Event Workflow Management Service" "python message passing client" "message passing" API mq apache pulsar pubsub rabbitmq pika nats nats.io OpenTelemetry tracing telemetry
 
 [metadata]
 name = oms-mqclient
 version = attr: mqclient.__version__
 url = https://github.com/Observation-Management-Service/MQClient
 author = WIPAC Developers
 author_email = developers@icecube.wisc.edu
@@ -19,17 +19,15 @@
 	Event Workflow Management Service
 	python message passing client
 	message passing
 	API
 	mq
 	apache
 	pulsar
-	google
 	pubsub
-	gcp
 	rabbitmq
 	pika
 	nats
 	nats.io
 	OpenTelemetry
 	tracing
 	telemetry
@@ -64,29 +62,23 @@
 install_requires = 
 	wipac-dev-tools
 
 [options.extras_require]
 all = 
 	%(pulsar)s
 	%(rabbitmq)s
-	%(gcp)s
 	%(nats)s
 pulsar = 
 	pulsar-client
 rabbitmq = 
 	pika
-gcp = 
-	google-api-core
-	google-auth
-	google-cloud-pubsub
-	googleapis-common-protos
 nats = 
 	nats-py[nkeys]
 telemetry = 
-	wipac-telemetry  # conflicts w/ gcp's reqs
+	wipac-telemetry
 dev = 
 	asyncstdlib
 	mypy
 	pytest
 	pytest-asyncio
 	pytest-mock
 	mock
```

### Comparing `oms-mqclient-1.2.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.0.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-1.2.0/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.0.0/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,16 +144,16 @@
             async with sub.open_sub() as gen:
                 recv_data_list = [m async for m in gen]
             return _log_recv_multiple(recv_data_list)
 
         def start_recv_thread(num_id: int) -> Any:
             return asyncio.run(recv_thread(num_id))
 
-        with ThreadPool(num_subs) as p:
-            received_data = p.map(start_recv_thread, range(num_subs))
+        with ThreadPool(num_subs) as pool:
+            received_data = pool.map(start_recv_thread, range(num_subs))
         all_recvd.extend(item for sublist in received_data for item in sublist)
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     async def test_21_fewer(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
@@ -199,16 +199,16 @@
             ).open_sub_one() as d:
                 recv_data = d
             return _log_recv(recv_data)
 
         def start_recv_thread(num_id: int) -> Any:
             return asyncio.run(recv_thread(num_id))
 
-        with ThreadPool(len(DATA_LIST)) as p:
-            all_recvd = p.map(start_recv_thread, range(len(DATA_LIST)))
+        with ThreadPool(len(DATA_LIST)) as pool:
+            all_recvd = pool.map(start_recv_thread, range(len(DATA_LIST)))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     async def test_23(self, queue_name: str, auth_token: str) -> None:
         """Failure-test one pub, and too many subs.
 
@@ -230,16 +230,16 @@
             ).open_sub_one() as d:
                 recv_data = d
             return _log_recv(recv_data)
 
         def start_recv_thread(num_id: int) -> Any:
             return asyncio.run(recv_thread(num_id))
 
-        with ThreadPool(len(DATA_LIST)) as p:
-            all_recvd = p.map(start_recv_thread, range(len(DATA_LIST)))
+        with ThreadPool(len(DATA_LIST)) as pool:
+            all_recvd = pool.map(start_recv_thread, range(len(DATA_LIST)))
 
         # Extra Sub
         with pytest.raises(Exception):
             await recv_thread(-1)
 
         assert all_were_received(all_recvd)
```

### Comparing `oms-mqclient-1.2.0/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.0.0/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-1.2.0/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.0.0/tests/abstract_broker_client_tests/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,15 @@
     obj_name = f"{obj.__class__.__module__}.{obj.__class__.__name__}"
 
     return obj_name == name or obj_name.endswith("." + name)
 
 
 @pytest.fixture
 def queue_name() -> str:
-    """Get random queue name.
-
-    Obeys the valid naming scheme for GCP (other broker_clients are less picky).
-    (See https://cloud.google.com/resource-manager/reference/rest/v1/projects#resource:-project)
-    """
+    """Get random queue name."""
     name = Queue.make_name()
     logging.info(f"NAME :: {name}")
     return name
 
 
 # Note: don't put in duplicates
 DATA_LIST = [
```

### Comparing `oms-mqclient-1.2.0/tests/integrate/conftest.py` & `oms-mqclient-2.0.0/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-1.2.0/tests/integrate/test_gcp.py` & `oms-mqclient-2.0.0/tests/integrate/test_pulsar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Run integration tests for GCP broker_client."""
+"""Run integration tests for Pulsar broker_client."""
 
 import logging
 
 from mqclient import broker_client_manager
 
 from ..abstract_broker_client_tests import (
     integrate_broker_client_interface,
@@ -12,19 +12,19 @@
     queue_name,
 )
 
 logging.getLogger().setLevel(logging.DEBUG)
 logging.getLogger("flake8").setLevel(logging.WARNING)
 
 
-class TestGCPQueue(integrate_queue.PubSubQueue):
-    """Run PubSubQueue integration tests with GCP broker_client."""
+class TestPulsarQueue(integrate_queue.PubSubQueue):
+    """Run PubSubQueue integration tests with Pulsar broker_client."""
 
-    broker_client = "gcp"
+    broker_client = "pulsar"
 
 
-class TestGCPBrokerClient(
+class TestPulsarBrokerClient(
     integrate_broker_client_interface.PubSubBrokerClientInterface
 ):
-    """Run PubSubBrokerClientInterface integration tests with GCP broker_client."""
+    """Run PubSubBrokerClientInterface integration tests with Pulsar broker_client."""
 
-    broker_client = broker_client_manager.get_broker_client("gcp")
+    broker_client = broker_client_manager.get_broker_client("pulsar")
```

### Comparing `oms-mqclient-1.2.0/tests/integrate/test_nats.py` & `oms-mqclient-2.0.0/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-1.2.0/tests/integrate/test_pulsar.py` & `oms-mqclient-2.0.0/tests/integrate/test_rabbitmq.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Run integration tests for Pulsar broker_client."""
+"""Run integration tests for RabbitMQ broker_client."""
 
 import logging
 
 from mqclient import broker_client_manager
 
 from ..abstract_broker_client_tests import (
     integrate_broker_client_interface,
@@ -10,21 +10,22 @@
 )
 from ..abstract_broker_client_tests.utils import (  # pytest.fixture # noqa: F401 # pylint: disable=W0611
     queue_name,
 )
 
 logging.getLogger().setLevel(logging.DEBUG)
 logging.getLogger("flake8").setLevel(logging.WARNING)
+logging.getLogger("pika").setLevel(logging.WARNING)
 
 
-class TestPulsarQueue(integrate_queue.PubSubQueue):
-    """Run PubSubQueue integration tests with Pulsar broker_client."""
+class TestRabbitMQQueue(integrate_queue.PubSubQueue):
+    """Run PubSubQueue integration tests with RabbitMQ broker_client."""
 
-    broker_client = "pulsar"
+    broker_client = "rabbitmq"
 
 
-class TestPulsarBrokerClient(
+class TestRabbitMQBrokerClient(
     integrate_broker_client_interface.PubSubBrokerClientInterface
 ):
-    """Run PubSubBrokerClientInterface integration tests with Pulsar broker_client."""
+    """Run PubSubBrokerClientInterface integration tests with RabbitMQ broker_client."""
 
-    broker_client = broker_client_manager.get_broker_client("pulsar")
+    broker_client = broker_client_manager.get_broker_client("rabbitmq")
```

### Comparing `oms-mqclient-1.2.0/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.0.0/tests/unit/pulsar/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-1.2.0/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.0.0/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files identical despite different names*

