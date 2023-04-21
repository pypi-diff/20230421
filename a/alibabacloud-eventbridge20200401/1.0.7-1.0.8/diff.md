# Comparing `tmp/alibabacloud_eventbridge20200401-1.0.7.tar.gz` & `tmp/alibabacloud_eventbridge20200401-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eventbridge20200401-1.0.7.tar", last modified: Thu Apr 13 01:46:35 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eventbridge20200401-1.0.8.tar", last modified: Fri Apr 21 03:40:55 2023, max compression
```

## Comparing `alibabacloud_eventbridge20200401-1.0.7.tar` & `alibabacloud_eventbridge20200401-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      351 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2376 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148087 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/client.py
--rw-r--r--   0 root         (0) root         (0)   733994 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2376 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      393 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   151575 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/client.py
+-rw-r--r--   0 root         (0) root         (0)   752295 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-21 03:40:55.000000 alibabacloud_eventbridge20200401-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-04-21 03:40:54.000000 alibabacloud_eventbridge20200401-1.0.8/setup.py
```

### Comparing `alibabacloud_eventbridge20200401-1.0.7/LICENSE` & `alibabacloud_eventbridge20200401-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-1.0.7/PKG-INFO` & `alibabacloud_eventbridge20200401-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eventbridge20200401
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud eventbridge (20200401) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eventbridge20200401-1.0.7/README-CN.md` & `alibabacloud_eventbridge20200401-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-1.0.7/README.md` & `alibabacloud_eventbridge20200401-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/client.py` & `alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,39 +305,47 @@
         runtime: util_models.RuntimeOptions,
     ) -> eventbridge_20200401_models.CreateEventSourceResponse:
         UtilClient.validate_model(tmp_req)
         request = eventbridge_20200401_models.CreateEventSourceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.source_http_event_parameters):
             request.source_http_event_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_http_event_parameters, 'SourceHttpEventParameters', 'json')
+        if not UtilClient.is_unset(tmp_req.source_kafka_parameters):
+            request.source_kafka_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_kafka_parameters, 'SourceKafkaParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_mnsparameters):
             request.source_mnsparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_mnsparameters, 'SourceMNSParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_rabbit_mqparameters):
             request.source_rabbit_mqparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_rabbit_mqparameters, 'SourceRabbitMQParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_rocket_mqparameters):
             request.source_rocket_mqparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_rocket_mqparameters, 'SourceRocketMQParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_slsparameters):
             request.source_slsparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_slsparameters, 'SourceSLSParameters', 'json')
+        if not UtilClient.is_unset(tmp_req.source_scheduled_event_parameters):
+            request.source_scheduled_event_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_scheduled_event_parameters, 'SourceScheduledEventParameters', 'json')
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.event_bus_name):
             body['EventBusName'] = request.event_bus_name
         if not UtilClient.is_unset(request.event_source_name):
             body['EventSourceName'] = request.event_source_name
         if not UtilClient.is_unset(request.source_http_event_parameters_shrink):
             body['SourceHttpEventParameters'] = request.source_http_event_parameters_shrink
+        if not UtilClient.is_unset(request.source_kafka_parameters_shrink):
+            body['SourceKafkaParameters'] = request.source_kafka_parameters_shrink
         if not UtilClient.is_unset(request.source_mnsparameters_shrink):
             body['SourceMNSParameters'] = request.source_mnsparameters_shrink
         if not UtilClient.is_unset(request.source_rabbit_mqparameters_shrink):
             body['SourceRabbitMQParameters'] = request.source_rabbit_mqparameters_shrink
         if not UtilClient.is_unset(request.source_rocket_mqparameters_shrink):
             body['SourceRocketMQParameters'] = request.source_rocket_mqparameters_shrink
         if not UtilClient.is_unset(request.source_slsparameters_shrink):
             body['SourceSLSParameters'] = request.source_slsparameters_shrink
+        if not UtilClient.is_unset(request.source_scheduled_event_parameters_shrink):
+            body['SourceScheduledEventParameters'] = request.source_scheduled_event_parameters_shrink
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateEventSource',
             version='2020-04-01',
             protocol='HTTPS',
@@ -359,39 +367,47 @@
         runtime: util_models.RuntimeOptions,
     ) -> eventbridge_20200401_models.CreateEventSourceResponse:
         UtilClient.validate_model(tmp_req)
         request = eventbridge_20200401_models.CreateEventSourceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.source_http_event_parameters):
             request.source_http_event_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_http_event_parameters, 'SourceHttpEventParameters', 'json')
+        if not UtilClient.is_unset(tmp_req.source_kafka_parameters):
+            request.source_kafka_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_kafka_parameters, 'SourceKafkaParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_mnsparameters):
             request.source_mnsparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_mnsparameters, 'SourceMNSParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_rabbit_mqparameters):
             request.source_rabbit_mqparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_rabbit_mqparameters, 'SourceRabbitMQParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_rocket_mqparameters):
             request.source_rocket_mqparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_rocket_mqparameters, 'SourceRocketMQParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_slsparameters):
             request.source_slsparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_slsparameters, 'SourceSLSParameters', 'json')
+        if not UtilClient.is_unset(tmp_req.source_scheduled_event_parameters):
+            request.source_scheduled_event_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_scheduled_event_parameters, 'SourceScheduledEventParameters', 'json')
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.event_bus_name):
             body['EventBusName'] = request.event_bus_name
         if not UtilClient.is_unset(request.event_source_name):
             body['EventSourceName'] = request.event_source_name
         if not UtilClient.is_unset(request.source_http_event_parameters_shrink):
             body['SourceHttpEventParameters'] = request.source_http_event_parameters_shrink
+        if not UtilClient.is_unset(request.source_kafka_parameters_shrink):
+            body['SourceKafkaParameters'] = request.source_kafka_parameters_shrink
         if not UtilClient.is_unset(request.source_mnsparameters_shrink):
             body['SourceMNSParameters'] = request.source_mnsparameters_shrink
         if not UtilClient.is_unset(request.source_rabbit_mqparameters_shrink):
             body['SourceRabbitMQParameters'] = request.source_rabbit_mqparameters_shrink
         if not UtilClient.is_unset(request.source_rocket_mqparameters_shrink):
             body['SourceRocketMQParameters'] = request.source_rocket_mqparameters_shrink
         if not UtilClient.is_unset(request.source_slsparameters_shrink):
             body['SourceSLSParameters'] = request.source_slsparameters_shrink
+        if not UtilClient.is_unset(request.source_scheduled_event_parameters_shrink):
+            body['SourceScheduledEventParameters'] = request.source_scheduled_event_parameters_shrink
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateEventSource',
             version='2020-04-01',
             protocol='HTTPS',
@@ -3179,39 +3195,47 @@
         runtime: util_models.RuntimeOptions,
     ) -> eventbridge_20200401_models.UpdateEventSourceResponse:
         UtilClient.validate_model(tmp_req)
         request = eventbridge_20200401_models.UpdateEventSourceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.source_http_event_parameters):
             request.source_http_event_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_http_event_parameters, 'SourceHttpEventParameters', 'json')
+        if not UtilClient.is_unset(tmp_req.source_kafka_parameters):
+            request.source_kafka_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_kafka_parameters, 'SourceKafkaParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_mnsparameters):
             request.source_mnsparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_mnsparameters, 'SourceMNSParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_rabbit_mqparameters):
             request.source_rabbit_mqparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_rabbit_mqparameters, 'SourceRabbitMQParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_rocket_mqparameters):
             request.source_rocket_mqparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_rocket_mqparameters, 'SourceRocketMQParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_slsparameters):
             request.source_slsparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_slsparameters, 'SourceSLSParameters', 'json')
+        if not UtilClient.is_unset(tmp_req.source_scheduled_event_parameters):
+            request.source_scheduled_event_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_scheduled_event_parameters, 'SourceScheduledEventParameters', 'json')
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.event_bus_name):
             body['EventBusName'] = request.event_bus_name
         if not UtilClient.is_unset(request.event_source_name):
             body['EventSourceName'] = request.event_source_name
         if not UtilClient.is_unset(request.source_http_event_parameters_shrink):
             body['SourceHttpEventParameters'] = request.source_http_event_parameters_shrink
+        if not UtilClient.is_unset(request.source_kafka_parameters_shrink):
+            body['SourceKafkaParameters'] = request.source_kafka_parameters_shrink
         if not UtilClient.is_unset(request.source_mnsparameters_shrink):
             body['SourceMNSParameters'] = request.source_mnsparameters_shrink
         if not UtilClient.is_unset(request.source_rabbit_mqparameters_shrink):
             body['SourceRabbitMQParameters'] = request.source_rabbit_mqparameters_shrink
         if not UtilClient.is_unset(request.source_rocket_mqparameters_shrink):
             body['SourceRocketMQParameters'] = request.source_rocket_mqparameters_shrink
         if not UtilClient.is_unset(request.source_slsparameters_shrink):
             body['SourceSLSParameters'] = request.source_slsparameters_shrink
+        if not UtilClient.is_unset(request.source_scheduled_event_parameters_shrink):
+            body['SourceScheduledEventParameters'] = request.source_scheduled_event_parameters_shrink
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateEventSource',
             version='2020-04-01',
             protocol='HTTPS',
@@ -3233,39 +3257,47 @@
         runtime: util_models.RuntimeOptions,
     ) -> eventbridge_20200401_models.UpdateEventSourceResponse:
         UtilClient.validate_model(tmp_req)
         request = eventbridge_20200401_models.UpdateEventSourceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.source_http_event_parameters):
             request.source_http_event_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_http_event_parameters, 'SourceHttpEventParameters', 'json')
+        if not UtilClient.is_unset(tmp_req.source_kafka_parameters):
+            request.source_kafka_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_kafka_parameters, 'SourceKafkaParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_mnsparameters):
             request.source_mnsparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_mnsparameters, 'SourceMNSParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_rabbit_mqparameters):
             request.source_rabbit_mqparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_rabbit_mqparameters, 'SourceRabbitMQParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_rocket_mqparameters):
             request.source_rocket_mqparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_rocket_mqparameters, 'SourceRocketMQParameters', 'json')
         if not UtilClient.is_unset(tmp_req.source_slsparameters):
             request.source_slsparameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_slsparameters, 'SourceSLSParameters', 'json')
+        if not UtilClient.is_unset(tmp_req.source_scheduled_event_parameters):
+            request.source_scheduled_event_parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.source_scheduled_event_parameters, 'SourceScheduledEventParameters', 'json')
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.event_bus_name):
             body['EventBusName'] = request.event_bus_name
         if not UtilClient.is_unset(request.event_source_name):
             body['EventSourceName'] = request.event_source_name
         if not UtilClient.is_unset(request.source_http_event_parameters_shrink):
             body['SourceHttpEventParameters'] = request.source_http_event_parameters_shrink
+        if not UtilClient.is_unset(request.source_kafka_parameters_shrink):
+            body['SourceKafkaParameters'] = request.source_kafka_parameters_shrink
         if not UtilClient.is_unset(request.source_mnsparameters_shrink):
             body['SourceMNSParameters'] = request.source_mnsparameters_shrink
         if not UtilClient.is_unset(request.source_rabbit_mqparameters_shrink):
             body['SourceRabbitMQParameters'] = request.source_rabbit_mqparameters_shrink
         if not UtilClient.is_unset(request.source_rocket_mqparameters_shrink):
             body['SourceRocketMQParameters'] = request.source_rocket_mqparameters_shrink
         if not UtilClient.is_unset(request.source_slsparameters_shrink):
             body['SourceSLSParameters'] = request.source_slsparameters_shrink
+        if not UtilClient.is_unset(request.source_scheduled_event_parameters_shrink):
+            body['SourceScheduledEventParameters'] = request.source_scheduled_event_parameters_shrink
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateEventSource',
             version='2020-04-01',
             protocol='HTTPS',
```

### Comparing `alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/models.py` & `alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1093,14 +1093,95 @@
         if m.get('SecurityConfig') is not None:
             self.security_config = m.get('SecurityConfig')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
+class CreateEventSourceRequestSourceKafkaParameters(TeaModel):
+    def __init__(
+        self,
+        consumer_group: str = None,
+        instance_id: str = None,
+        maximum_tasks: int = None,
+        network: str = None,
+        offset_reset: str = None,
+        region_id: str = None,
+        security_group_id: str = None,
+        topic: str = None,
+        v_switch_ids: str = None,
+        vpc_id: str = None,
+    ):
+        self.consumer_group = consumer_group
+        self.instance_id = instance_id
+        self.maximum_tasks = maximum_tasks
+        self.network = network
+        self.offset_reset = offset_reset
+        self.region_id = region_id
+        self.security_group_id = security_group_id
+        self.topic = topic
+        self.v_switch_ids = v_switch_ids
+        self.vpc_id = vpc_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.consumer_group is not None:
+            result['ConsumerGroup'] = self.consumer_group
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.maximum_tasks is not None:
+            result['MaximumTasks'] = self.maximum_tasks
+        if self.network is not None:
+            result['Network'] = self.network
+        if self.offset_reset is not None:
+            result['OffsetReset'] = self.offset_reset
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.security_group_id is not None:
+            result['SecurityGroupId'] = self.security_group_id
+        if self.topic is not None:
+            result['Topic'] = self.topic
+        if self.v_switch_ids is not None:
+            result['VSwitchIds'] = self.v_switch_ids
+        if self.vpc_id is not None:
+            result['VpcId'] = self.vpc_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ConsumerGroup') is not None:
+            self.consumer_group = m.get('ConsumerGroup')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MaximumTasks') is not None:
+            self.maximum_tasks = m.get('MaximumTasks')
+        if m.get('Network') is not None:
+            self.network = m.get('Network')
+        if m.get('OffsetReset') is not None:
+            self.offset_reset = m.get('OffsetReset')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('SecurityGroupId') is not None:
+            self.security_group_id = m.get('SecurityGroupId')
+        if m.get('Topic') is not None:
+            self.topic = m.get('Topic')
+        if m.get('VSwitchIds') is not None:
+            self.v_switch_ids = m.get('VSwitchIds')
+        if m.get('VpcId') is not None:
+            self.vpc_id = m.get('VpcId')
+        return self
+
+
 class CreateEventSourceRequestSourceMNSParameters(TeaModel):
     def __init__(
         self,
         is_base_64decode: str = None,
         queue_name: str = None,
         region_id: str = None,
     ):
@@ -1315,49 +1396,90 @@
         if m.get('Project') is not None:
             self.project = m.get('Project')
         if m.get('RoleName') is not None:
             self.role_name = m.get('RoleName')
         return self
 
 
+class CreateEventSourceRequestSourceScheduledEventParameters(TeaModel):
+    def __init__(
+        self,
+        schedule: str = None,
+        time_zone: str = None,
+    ):
+        self.schedule = schedule
+        self.time_zone = time_zone
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.schedule is not None:
+            result['Schedule'] = self.schedule
+        if self.time_zone is not None:
+            result['TimeZone'] = self.time_zone
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Schedule') is not None:
+            self.schedule = m.get('Schedule')
+        if m.get('TimeZone') is not None:
+            self.time_zone = m.get('TimeZone')
+        return self
+
+
 class CreateEventSourceRequest(TeaModel):
     def __init__(
         self,
-        description: bytes = None,
-        event_bus_name: bytes = None,
-        event_source_name: bytes = None,
+        description: str = None,
+        event_bus_name: str = None,
+        event_source_name: str = None,
         source_http_event_parameters: CreateEventSourceRequestSourceHttpEventParameters = None,
+        source_kafka_parameters: CreateEventSourceRequestSourceKafkaParameters = None,
         source_mnsparameters: CreateEventSourceRequestSourceMNSParameters = None,
         source_rabbit_mqparameters: CreateEventSourceRequestSourceRabbitMQParameters = None,
         source_rocket_mqparameters: CreateEventSourceRequestSourceRocketMQParameters = None,
         source_slsparameters: CreateEventSourceRequestSourceSLSParameters = None,
+        source_scheduled_event_parameters: CreateEventSourceRequestSourceScheduledEventParameters = None,
     ):
         # 事件源描述详情
         self.description = description
         self.event_bus_name = event_bus_name
         # 事件源英文Code
         self.event_source_name = event_source_name
         self.source_http_event_parameters = source_http_event_parameters
+        self.source_kafka_parameters = source_kafka_parameters
         self.source_mnsparameters = source_mnsparameters
         self.source_rabbit_mqparameters = source_rabbit_mqparameters
         self.source_rocket_mqparameters = source_rocket_mqparameters
         # SourceSLSParameters
         self.source_slsparameters = source_slsparameters
+        self.source_scheduled_event_parameters = source_scheduled_event_parameters
 
     def validate(self):
         if self.source_http_event_parameters:
             self.source_http_event_parameters.validate()
+        if self.source_kafka_parameters:
+            self.source_kafka_parameters.validate()
         if self.source_mnsparameters:
             self.source_mnsparameters.validate()
         if self.source_rabbit_mqparameters:
             self.source_rabbit_mqparameters.validate()
         if self.source_rocket_mqparameters:
             self.source_rocket_mqparameters.validate()
         if self.source_slsparameters:
             self.source_slsparameters.validate()
+        if self.source_scheduled_event_parameters:
+            self.source_scheduled_event_parameters.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1365,73 +1487,87 @@
             result['Description'] = self.description
         if self.event_bus_name is not None:
             result['EventBusName'] = self.event_bus_name
         if self.event_source_name is not None:
             result['EventSourceName'] = self.event_source_name
         if self.source_http_event_parameters is not None:
             result['SourceHttpEventParameters'] = self.source_http_event_parameters.to_map()
+        if self.source_kafka_parameters is not None:
+            result['SourceKafkaParameters'] = self.source_kafka_parameters.to_map()
         if self.source_mnsparameters is not None:
             result['SourceMNSParameters'] = self.source_mnsparameters.to_map()
         if self.source_rabbit_mqparameters is not None:
             result['SourceRabbitMQParameters'] = self.source_rabbit_mqparameters.to_map()
         if self.source_rocket_mqparameters is not None:
             result['SourceRocketMQParameters'] = self.source_rocket_mqparameters.to_map()
         if self.source_slsparameters is not None:
             result['SourceSLSParameters'] = self.source_slsparameters.to_map()
+        if self.source_scheduled_event_parameters is not None:
+            result['SourceScheduledEventParameters'] = self.source_scheduled_event_parameters.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('EventBusName') is not None:
             self.event_bus_name = m.get('EventBusName')
         if m.get('EventSourceName') is not None:
             self.event_source_name = m.get('EventSourceName')
         if m.get('SourceHttpEventParameters') is not None:
             temp_model = CreateEventSourceRequestSourceHttpEventParameters()
             self.source_http_event_parameters = temp_model.from_map(m['SourceHttpEventParameters'])
+        if m.get('SourceKafkaParameters') is not None:
+            temp_model = CreateEventSourceRequestSourceKafkaParameters()
+            self.source_kafka_parameters = temp_model.from_map(m['SourceKafkaParameters'])
         if m.get('SourceMNSParameters') is not None:
             temp_model = CreateEventSourceRequestSourceMNSParameters()
             self.source_mnsparameters = temp_model.from_map(m['SourceMNSParameters'])
         if m.get('SourceRabbitMQParameters') is not None:
             temp_model = CreateEventSourceRequestSourceRabbitMQParameters()
             self.source_rabbit_mqparameters = temp_model.from_map(m['SourceRabbitMQParameters'])
         if m.get('SourceRocketMQParameters') is not None:
             temp_model = CreateEventSourceRequestSourceRocketMQParameters()
             self.source_rocket_mqparameters = temp_model.from_map(m['SourceRocketMQParameters'])
         if m.get('SourceSLSParameters') is not None:
             temp_model = CreateEventSourceRequestSourceSLSParameters()
             self.source_slsparameters = temp_model.from_map(m['SourceSLSParameters'])
+        if m.get('SourceScheduledEventParameters') is not None:
+            temp_model = CreateEventSourceRequestSourceScheduledEventParameters()
+            self.source_scheduled_event_parameters = temp_model.from_map(m['SourceScheduledEventParameters'])
         return self
 
 
 class CreateEventSourceShrinkRequest(TeaModel):
     def __init__(
         self,
-        description: bytes = None,
-        event_bus_name: bytes = None,
-        event_source_name: bytes = None,
+        description: str = None,
+        event_bus_name: str = None,
+        event_source_name: str = None,
         source_http_event_parameters_shrink: str = None,
+        source_kafka_parameters_shrink: str = None,
         source_mnsparameters_shrink: str = None,
         source_rabbit_mqparameters_shrink: str = None,
         source_rocket_mqparameters_shrink: str = None,
         source_slsparameters_shrink: str = None,
+        source_scheduled_event_parameters_shrink: str = None,
     ):
         # 事件源描述详情
         self.description = description
         self.event_bus_name = event_bus_name
         # 事件源英文Code
         self.event_source_name = event_source_name
         self.source_http_event_parameters_shrink = source_http_event_parameters_shrink
+        self.source_kafka_parameters_shrink = source_kafka_parameters_shrink
         self.source_mnsparameters_shrink = source_mnsparameters_shrink
         self.source_rabbit_mqparameters_shrink = source_rabbit_mqparameters_shrink
         self.source_rocket_mqparameters_shrink = source_rocket_mqparameters_shrink
         # SourceSLSParameters
         self.source_slsparameters_shrink = source_slsparameters_shrink
+        self.source_scheduled_event_parameters_shrink = source_scheduled_event_parameters_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1442,42 +1578,50 @@
             result['Description'] = self.description
         if self.event_bus_name is not None:
             result['EventBusName'] = self.event_bus_name
         if self.event_source_name is not None:
             result['EventSourceName'] = self.event_source_name
         if self.source_http_event_parameters_shrink is not None:
             result['SourceHttpEventParameters'] = self.source_http_event_parameters_shrink
+        if self.source_kafka_parameters_shrink is not None:
+            result['SourceKafkaParameters'] = self.source_kafka_parameters_shrink
         if self.source_mnsparameters_shrink is not None:
             result['SourceMNSParameters'] = self.source_mnsparameters_shrink
         if self.source_rabbit_mqparameters_shrink is not None:
             result['SourceRabbitMQParameters'] = self.source_rabbit_mqparameters_shrink
         if self.source_rocket_mqparameters_shrink is not None:
             result['SourceRocketMQParameters'] = self.source_rocket_mqparameters_shrink
         if self.source_slsparameters_shrink is not None:
             result['SourceSLSParameters'] = self.source_slsparameters_shrink
+        if self.source_scheduled_event_parameters_shrink is not None:
+            result['SourceScheduledEventParameters'] = self.source_scheduled_event_parameters_shrink
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('EventBusName') is not None:
             self.event_bus_name = m.get('EventBusName')
         if m.get('EventSourceName') is not None:
             self.event_source_name = m.get('EventSourceName')
         if m.get('SourceHttpEventParameters') is not None:
             self.source_http_event_parameters_shrink = m.get('SourceHttpEventParameters')
+        if m.get('SourceKafkaParameters') is not None:
+            self.source_kafka_parameters_shrink = m.get('SourceKafkaParameters')
         if m.get('SourceMNSParameters') is not None:
             self.source_mnsparameters_shrink = m.get('SourceMNSParameters')
         if m.get('SourceRabbitMQParameters') is not None:
             self.source_rabbit_mqparameters_shrink = m.get('SourceRabbitMQParameters')
         if m.get('SourceRocketMQParameters') is not None:
             self.source_rocket_mqparameters_shrink = m.get('SourceRocketMQParameters')
         if m.get('SourceSLSParameters') is not None:
             self.source_slsparameters_shrink = m.get('SourceSLSParameters')
+        if m.get('SourceScheduledEventParameters') is not None:
+            self.source_scheduled_event_parameters_shrink = m.get('SourceScheduledEventParameters')
         return self
 
 
 class CreateEventSourceResponseBodyData(TeaModel):
     def __init__(
         self,
         event_source_arn: str = None,
@@ -2102,14 +2246,53 @@
         if m.get('Template') is not None:
             self.template = m.get('Template')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
+class CreateEventStreamingRequestSinkSinkFcParametersConcurrency(TeaModel):
+    def __init__(
+        self,
+        form: str = None,
+        template: str = None,
+        value: str = None,
+    ):
+        self.form = form
+        self.template = template
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.form is not None:
+            result['Form'] = self.form
+        if self.template is not None:
+            result['Template'] = self.template
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Form') is not None:
+            self.form = m.get('Form')
+        if m.get('Template') is not None:
+            self.template = m.get('Template')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateEventStreamingRequestSinkSinkFcParametersFunctionName(TeaModel):
     def __init__(
         self,
         form: str = None,
         template: str = None,
         value: str = None,
     ):
@@ -2262,28 +2445,32 @@
         return self
 
 
 class CreateEventStreamingRequestSinkSinkFcParameters(TeaModel):
     def __init__(
         self,
         body: CreateEventStreamingRequestSinkSinkFcParametersBody = None,
+        concurrency: CreateEventStreamingRequestSinkSinkFcParametersConcurrency = None,
         function_name: CreateEventStreamingRequestSinkSinkFcParametersFunctionName = None,
         invocation_type: CreateEventStreamingRequestSinkSinkFcParametersInvocationType = None,
         qualifier: CreateEventStreamingRequestSinkSinkFcParametersQualifier = None,
         service_name: CreateEventStreamingRequestSinkSinkFcParametersServiceName = None,
     ):
         self.body = body
+        self.concurrency = concurrency
         self.function_name = function_name
         self.invocation_type = invocation_type
         self.qualifier = qualifier
         self.service_name = service_name
 
     def validate(self):
         if self.body:
             self.body.validate()
+        if self.concurrency:
+            self.concurrency.validate()
         if self.function_name:
             self.function_name.validate()
         if self.invocation_type:
             self.invocation_type.validate()
         if self.qualifier:
             self.qualifier.validate()
         if self.service_name:
@@ -2293,14 +2480,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.body is not None:
             result['Body'] = self.body.to_map()
+        if self.concurrency is not None:
+            result['Concurrency'] = self.concurrency.to_map()
         if self.function_name is not None:
             result['FunctionName'] = self.function_name.to_map()
         if self.invocation_type is not None:
             result['InvocationType'] = self.invocation_type.to_map()
         if self.qualifier is not None:
             result['Qualifier'] = self.qualifier.to_map()
         if self.service_name is not None:
@@ -2308,14 +2497,17 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Body') is not None:
             temp_model = CreateEventStreamingRequestSinkSinkFcParametersBody()
             self.body = temp_model.from_map(m['Body'])
+        if m.get('Concurrency') is not None:
+            temp_model = CreateEventStreamingRequestSinkSinkFcParametersConcurrency()
+            self.concurrency = temp_model.from_map(m['Concurrency'])
         if m.get('FunctionName') is not None:
             temp_model = CreateEventStreamingRequestSinkSinkFcParametersFunctionName()
             self.function_name = temp_model.from_map(m['FunctionName'])
         if m.get('InvocationType') is not None:
             temp_model = CreateEventStreamingRequestSinkSinkFcParametersInvocationType()
             self.invocation_type = temp_model.from_map(m['InvocationType'])
         if m.get('Qualifier') is not None:
@@ -8546,14 +8738,53 @@
         if m.get('Template') is not None:
             self.template = m.get('Template')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
+class GetEventStreamingResponseBodyDataSinkSinkFcParametersConcurrency(TeaModel):
+    def __init__(
+        self,
+        form: str = None,
+        template: str = None,
+        value: str = None,
+    ):
+        self.form = form
+        self.template = template
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.form is not None:
+            result['Form'] = self.form
+        if self.template is not None:
+            result['Template'] = self.template
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Form') is not None:
+            self.form = m.get('Form')
+        if m.get('Template') is not None:
+            self.template = m.get('Template')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class GetEventStreamingResponseBodyDataSinkSinkFcParametersFunctionName(TeaModel):
     def __init__(
         self,
         form: str = None,
         template: str = None,
         value: str = None,
     ):
@@ -8706,28 +8937,32 @@
         return self
 
 
 class GetEventStreamingResponseBodyDataSinkSinkFcParameters(TeaModel):
     def __init__(
         self,
         body: GetEventStreamingResponseBodyDataSinkSinkFcParametersBody = None,
+        concurrency: GetEventStreamingResponseBodyDataSinkSinkFcParametersConcurrency = None,
         function_name: GetEventStreamingResponseBodyDataSinkSinkFcParametersFunctionName = None,
         invocation_type: GetEventStreamingResponseBodyDataSinkSinkFcParametersInvocationType = None,
         qualifier: GetEventStreamingResponseBodyDataSinkSinkFcParametersQualifier = None,
         service_name: GetEventStreamingResponseBodyDataSinkSinkFcParametersServiceName = None,
     ):
         self.body = body
+        self.concurrency = concurrency
         self.function_name = function_name
         self.invocation_type = invocation_type
         self.qualifier = qualifier
         self.service_name = service_name
 
     def validate(self):
         if self.body:
             self.body.validate()
+        if self.concurrency:
+            self.concurrency.validate()
         if self.function_name:
             self.function_name.validate()
         if self.invocation_type:
             self.invocation_type.validate()
         if self.qualifier:
             self.qualifier.validate()
         if self.service_name:
@@ -8737,14 +8972,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.body is not None:
             result['Body'] = self.body.to_map()
+        if self.concurrency is not None:
+            result['Concurrency'] = self.concurrency.to_map()
         if self.function_name is not None:
             result['FunctionName'] = self.function_name.to_map()
         if self.invocation_type is not None:
             result['InvocationType'] = self.invocation_type.to_map()
         if self.qualifier is not None:
             result['Qualifier'] = self.qualifier.to_map()
         if self.service_name is not None:
@@ -8752,14 +8989,17 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Body') is not None:
             temp_model = GetEventStreamingResponseBodyDataSinkSinkFcParametersBody()
             self.body = temp_model.from_map(m['Body'])
+        if m.get('Concurrency') is not None:
+            temp_model = GetEventStreamingResponseBodyDataSinkSinkFcParametersConcurrency()
+            self.concurrency = temp_model.from_map(m['Concurrency'])
         if m.get('FunctionName') is not None:
             temp_model = GetEventStreamingResponseBodyDataSinkSinkFcParametersFunctionName()
             self.function_name = temp_model.from_map(m['FunctionName'])
         if m.get('InvocationType') is not None:
             temp_model = GetEventStreamingResponseBodyDataSinkSinkFcParametersInvocationType()
             self.invocation_type = temp_model.from_map(m['InvocationType'])
         if m.get('Qualifier') is not None:
@@ -13124,14 +13364,53 @@
         if m.get('Template') is not None:
             self.template = m.get('Template')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
+class ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersConcurrency(TeaModel):
+    def __init__(
+        self,
+        form: str = None,
+        template: str = None,
+        value: str = None,
+    ):
+        self.form = form
+        self.template = template
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.form is not None:
+            result['Form'] = self.form
+        if self.template is not None:
+            result['Template'] = self.template
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Form') is not None:
+            self.form = m.get('Form')
+        if m.get('Template') is not None:
+            self.template = m.get('Template')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersFunctionName(TeaModel):
     def __init__(
         self,
         form: str = None,
         template: str = None,
         value: str = None,
     ):
@@ -13284,28 +13563,32 @@
         return self
 
 
 class ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParameters(TeaModel):
     def __init__(
         self,
         body: ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersBody = None,
+        concurrency: ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersConcurrency = None,
         function_name: ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersFunctionName = None,
         invocation_type: ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersInvocationType = None,
         qualifier: ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersQualifier = None,
         service_name: ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersServiceName = None,
     ):
         self.body = body
+        self.concurrency = concurrency
         self.function_name = function_name
         self.invocation_type = invocation_type
         self.qualifier = qualifier
         self.service_name = service_name
 
     def validate(self):
         if self.body:
             self.body.validate()
+        if self.concurrency:
+            self.concurrency.validate()
         if self.function_name:
             self.function_name.validate()
         if self.invocation_type:
             self.invocation_type.validate()
         if self.qualifier:
             self.qualifier.validate()
         if self.service_name:
@@ -13315,14 +13598,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.body is not None:
             result['Body'] = self.body.to_map()
+        if self.concurrency is not None:
+            result['Concurrency'] = self.concurrency.to_map()
         if self.function_name is not None:
             result['FunctionName'] = self.function_name.to_map()
         if self.invocation_type is not None:
             result['InvocationType'] = self.invocation_type.to_map()
         if self.qualifier is not None:
             result['Qualifier'] = self.qualifier.to_map()
         if self.service_name is not None:
@@ -13330,14 +13615,17 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Body') is not None:
             temp_model = ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersBody()
             self.body = temp_model.from_map(m['Body'])
+        if m.get('Concurrency') is not None:
+            temp_model = ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersConcurrency()
+            self.concurrency = temp_model.from_map(m['Concurrency'])
         if m.get('FunctionName') is not None:
             temp_model = ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersFunctionName()
             self.function_name = temp_model.from_map(m['FunctionName'])
         if m.get('InvocationType') is not None:
             temp_model = ListEventStreamingsResponseBodyDataEventStreamingsSinkSinkFcParametersInvocationType()
             self.invocation_type = temp_model.from_map(m['InvocationType'])
         if m.get('Qualifier') is not None:
@@ -18996,14 +19284,95 @@
         if m.get('SecurityConfig') is not None:
             self.security_config = m.get('SecurityConfig')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
+class UpdateEventSourceRequestSourceKafkaParameters(TeaModel):
+    def __init__(
+        self,
+        consumer_group: str = None,
+        instance_id: str = None,
+        maximum_tasks: int = None,
+        network: str = None,
+        offset_reset: str = None,
+        region_id: str = None,
+        security_group_id: str = None,
+        topic: str = None,
+        v_switch_ids: str = None,
+        vpc_id: str = None,
+    ):
+        self.consumer_group = consumer_group
+        self.instance_id = instance_id
+        self.maximum_tasks = maximum_tasks
+        self.network = network
+        self.offset_reset = offset_reset
+        self.region_id = region_id
+        self.security_group_id = security_group_id
+        self.topic = topic
+        self.v_switch_ids = v_switch_ids
+        self.vpc_id = vpc_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.consumer_group is not None:
+            result['ConsumerGroup'] = self.consumer_group
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.maximum_tasks is not None:
+            result['MaximumTasks'] = self.maximum_tasks
+        if self.network is not None:
+            result['Network'] = self.network
+        if self.offset_reset is not None:
+            result['OffsetReset'] = self.offset_reset
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.security_group_id is not None:
+            result['SecurityGroupId'] = self.security_group_id
+        if self.topic is not None:
+            result['Topic'] = self.topic
+        if self.v_switch_ids is not None:
+            result['VSwitchIds'] = self.v_switch_ids
+        if self.vpc_id is not None:
+            result['VpcId'] = self.vpc_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ConsumerGroup') is not None:
+            self.consumer_group = m.get('ConsumerGroup')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MaximumTasks') is not None:
+            self.maximum_tasks = m.get('MaximumTasks')
+        if m.get('Network') is not None:
+            self.network = m.get('Network')
+        if m.get('OffsetReset') is not None:
+            self.offset_reset = m.get('OffsetReset')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('SecurityGroupId') is not None:
+            self.security_group_id = m.get('SecurityGroupId')
+        if m.get('Topic') is not None:
+            self.topic = m.get('Topic')
+        if m.get('VSwitchIds') is not None:
+            self.v_switch_ids = m.get('VSwitchIds')
+        if m.get('VpcId') is not None:
+            self.vpc_id = m.get('VpcId')
+        return self
+
+
 class UpdateEventSourceRequestSourceMNSParameters(TeaModel):
     def __init__(
         self,
         is_base_64decode: str = None,
         queue_name: str = None,
         region_id: str = None,
     ):
@@ -19218,49 +19587,90 @@
         if m.get('Project') is not None:
             self.project = m.get('Project')
         if m.get('RoleName') is not None:
             self.role_name = m.get('RoleName')
         return self
 
 
+class UpdateEventSourceRequestSourceScheduledEventParameters(TeaModel):
+    def __init__(
+        self,
+        schedule: str = None,
+        time_zone: str = None,
+    ):
+        self.schedule = schedule
+        self.time_zone = time_zone
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.schedule is not None:
+            result['Schedule'] = self.schedule
+        if self.time_zone is not None:
+            result['TimeZone'] = self.time_zone
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Schedule') is not None:
+            self.schedule = m.get('Schedule')
+        if m.get('TimeZone') is not None:
+            self.time_zone = m.get('TimeZone')
+        return self
+
+
 class UpdateEventSourceRequest(TeaModel):
     def __init__(
         self,
-        description: bytes = None,
+        description: str = None,
         event_bus_name: bytes = None,
-        event_source_name: bytes = None,
+        event_source_name: str = None,
         source_http_event_parameters: UpdateEventSourceRequestSourceHttpEventParameters = None,
+        source_kafka_parameters: UpdateEventSourceRequestSourceKafkaParameters = None,
         source_mnsparameters: UpdateEventSourceRequestSourceMNSParameters = None,
         source_rabbit_mqparameters: UpdateEventSourceRequestSourceRabbitMQParameters = None,
         source_rocket_mqparameters: UpdateEventSourceRequestSourceRocketMQParameters = None,
         source_slsparameters: UpdateEventSourceRequestSourceSLSParameters = None,
+        source_scheduled_event_parameters: UpdateEventSourceRequestSourceScheduledEventParameters = None,
     ):
         # 事件源描述详情
         self.description = description
         self.event_bus_name = event_bus_name
         # 事件源英文Code
         self.event_source_name = event_source_name
         self.source_http_event_parameters = source_http_event_parameters
+        self.source_kafka_parameters = source_kafka_parameters
         self.source_mnsparameters = source_mnsparameters
         self.source_rabbit_mqparameters = source_rabbit_mqparameters
         self.source_rocket_mqparameters = source_rocket_mqparameters
         # SourceSLSParameters
         self.source_slsparameters = source_slsparameters
+        self.source_scheduled_event_parameters = source_scheduled_event_parameters
 
     def validate(self):
         if self.source_http_event_parameters:
             self.source_http_event_parameters.validate()
+        if self.source_kafka_parameters:
+            self.source_kafka_parameters.validate()
         if self.source_mnsparameters:
             self.source_mnsparameters.validate()
         if self.source_rabbit_mqparameters:
             self.source_rabbit_mqparameters.validate()
         if self.source_rocket_mqparameters:
             self.source_rocket_mqparameters.validate()
         if self.source_slsparameters:
             self.source_slsparameters.validate()
+        if self.source_scheduled_event_parameters:
+            self.source_scheduled_event_parameters.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -19268,73 +19678,87 @@
             result['Description'] = self.description
         if self.event_bus_name is not None:
             result['EventBusName'] = self.event_bus_name
         if self.event_source_name is not None:
             result['EventSourceName'] = self.event_source_name
         if self.source_http_event_parameters is not None:
             result['SourceHttpEventParameters'] = self.source_http_event_parameters.to_map()
+        if self.source_kafka_parameters is not None:
+            result['SourceKafkaParameters'] = self.source_kafka_parameters.to_map()
         if self.source_mnsparameters is not None:
             result['SourceMNSParameters'] = self.source_mnsparameters.to_map()
         if self.source_rabbit_mqparameters is not None:
             result['SourceRabbitMQParameters'] = self.source_rabbit_mqparameters.to_map()
         if self.source_rocket_mqparameters is not None:
             result['SourceRocketMQParameters'] = self.source_rocket_mqparameters.to_map()
         if self.source_slsparameters is not None:
             result['SourceSLSParameters'] = self.source_slsparameters.to_map()
+        if self.source_scheduled_event_parameters is not None:
+            result['SourceScheduledEventParameters'] = self.source_scheduled_event_parameters.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('EventBusName') is not None:
             self.event_bus_name = m.get('EventBusName')
         if m.get('EventSourceName') is not None:
             self.event_source_name = m.get('EventSourceName')
         if m.get('SourceHttpEventParameters') is not None:
             temp_model = UpdateEventSourceRequestSourceHttpEventParameters()
             self.source_http_event_parameters = temp_model.from_map(m['SourceHttpEventParameters'])
+        if m.get('SourceKafkaParameters') is not None:
+            temp_model = UpdateEventSourceRequestSourceKafkaParameters()
+            self.source_kafka_parameters = temp_model.from_map(m['SourceKafkaParameters'])
         if m.get('SourceMNSParameters') is not None:
             temp_model = UpdateEventSourceRequestSourceMNSParameters()
             self.source_mnsparameters = temp_model.from_map(m['SourceMNSParameters'])
         if m.get('SourceRabbitMQParameters') is not None:
             temp_model = UpdateEventSourceRequestSourceRabbitMQParameters()
             self.source_rabbit_mqparameters = temp_model.from_map(m['SourceRabbitMQParameters'])
         if m.get('SourceRocketMQParameters') is not None:
             temp_model = UpdateEventSourceRequestSourceRocketMQParameters()
             self.source_rocket_mqparameters = temp_model.from_map(m['SourceRocketMQParameters'])
         if m.get('SourceSLSParameters') is not None:
             temp_model = UpdateEventSourceRequestSourceSLSParameters()
             self.source_slsparameters = temp_model.from_map(m['SourceSLSParameters'])
+        if m.get('SourceScheduledEventParameters') is not None:
+            temp_model = UpdateEventSourceRequestSourceScheduledEventParameters()
+            self.source_scheduled_event_parameters = temp_model.from_map(m['SourceScheduledEventParameters'])
         return self
 
 
 class UpdateEventSourceShrinkRequest(TeaModel):
     def __init__(
         self,
-        description: bytes = None,
+        description: str = None,
         event_bus_name: bytes = None,
-        event_source_name: bytes = None,
+        event_source_name: str = None,
         source_http_event_parameters_shrink: str = None,
+        source_kafka_parameters_shrink: str = None,
         source_mnsparameters_shrink: str = None,
         source_rabbit_mqparameters_shrink: str = None,
         source_rocket_mqparameters_shrink: str = None,
         source_slsparameters_shrink: str = None,
+        source_scheduled_event_parameters_shrink: str = None,
     ):
         # 事件源描述详情
         self.description = description
         self.event_bus_name = event_bus_name
         # 事件源英文Code
         self.event_source_name = event_source_name
         self.source_http_event_parameters_shrink = source_http_event_parameters_shrink
+        self.source_kafka_parameters_shrink = source_kafka_parameters_shrink
         self.source_mnsparameters_shrink = source_mnsparameters_shrink
         self.source_rabbit_mqparameters_shrink = source_rabbit_mqparameters_shrink
         self.source_rocket_mqparameters_shrink = source_rocket_mqparameters_shrink
         # SourceSLSParameters
         self.source_slsparameters_shrink = source_slsparameters_shrink
+        self.source_scheduled_event_parameters_shrink = source_scheduled_event_parameters_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -19345,42 +19769,50 @@
             result['Description'] = self.description
         if self.event_bus_name is not None:
             result['EventBusName'] = self.event_bus_name
         if self.event_source_name is not None:
             result['EventSourceName'] = self.event_source_name
         if self.source_http_event_parameters_shrink is not None:
             result['SourceHttpEventParameters'] = self.source_http_event_parameters_shrink
+        if self.source_kafka_parameters_shrink is not None:
+            result['SourceKafkaParameters'] = self.source_kafka_parameters_shrink
         if self.source_mnsparameters_shrink is not None:
             result['SourceMNSParameters'] = self.source_mnsparameters_shrink
         if self.source_rabbit_mqparameters_shrink is not None:
             result['SourceRabbitMQParameters'] = self.source_rabbit_mqparameters_shrink
         if self.source_rocket_mqparameters_shrink is not None:
             result['SourceRocketMQParameters'] = self.source_rocket_mqparameters_shrink
         if self.source_slsparameters_shrink is not None:
             result['SourceSLSParameters'] = self.source_slsparameters_shrink
+        if self.source_scheduled_event_parameters_shrink is not None:
+            result['SourceScheduledEventParameters'] = self.source_scheduled_event_parameters_shrink
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('EventBusName') is not None:
             self.event_bus_name = m.get('EventBusName')
         if m.get('EventSourceName') is not None:
             self.event_source_name = m.get('EventSourceName')
         if m.get('SourceHttpEventParameters') is not None:
             self.source_http_event_parameters_shrink = m.get('SourceHttpEventParameters')
+        if m.get('SourceKafkaParameters') is not None:
+            self.source_kafka_parameters_shrink = m.get('SourceKafkaParameters')
         if m.get('SourceMNSParameters') is not None:
             self.source_mnsparameters_shrink = m.get('SourceMNSParameters')
         if m.get('SourceRabbitMQParameters') is not None:
             self.source_rabbit_mqparameters_shrink = m.get('SourceRabbitMQParameters')
         if m.get('SourceRocketMQParameters') is not None:
             self.source_rocket_mqparameters_shrink = m.get('SourceRocketMQParameters')
         if m.get('SourceSLSParameters') is not None:
             self.source_slsparameters_shrink = m.get('SourceSLSParameters')
+        if m.get('SourceScheduledEventParameters') is not None:
+            self.source_scheduled_event_parameters_shrink = m.get('SourceScheduledEventParameters')
         return self
 
 
 class UpdateEventSourceResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
@@ -19668,14 +20100,53 @@
         if m.get('Template') is not None:
             self.template = m.get('Template')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
+class UpdateEventStreamingRequestSinkSinkFcParametersConcurrency(TeaModel):
+    def __init__(
+        self,
+        form: str = None,
+        template: str = None,
+        value: str = None,
+    ):
+        self.form = form
+        self.template = template
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.form is not None:
+            result['Form'] = self.form
+        if self.template is not None:
+            result['Template'] = self.template
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Form') is not None:
+            self.form = m.get('Form')
+        if m.get('Template') is not None:
+            self.template = m.get('Template')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class UpdateEventStreamingRequestSinkSinkFcParametersFunctionName(TeaModel):
     def __init__(
         self,
         form: str = None,
         template: str = None,
         value: str = None,
     ):
@@ -19828,28 +20299,32 @@
         return self
 
 
 class UpdateEventStreamingRequestSinkSinkFcParameters(TeaModel):
     def __init__(
         self,
         body: UpdateEventStreamingRequestSinkSinkFcParametersBody = None,
+        concurrency: UpdateEventStreamingRequestSinkSinkFcParametersConcurrency = None,
         function_name: UpdateEventStreamingRequestSinkSinkFcParametersFunctionName = None,
         invocation_type: UpdateEventStreamingRequestSinkSinkFcParametersInvocationType = None,
         qualifier: UpdateEventStreamingRequestSinkSinkFcParametersQualifier = None,
         service_name: UpdateEventStreamingRequestSinkSinkFcParametersServiceName = None,
     ):
         self.body = body
+        self.concurrency = concurrency
         self.function_name = function_name
         self.invocation_type = invocation_type
         self.qualifier = qualifier
         self.service_name = service_name
 
     def validate(self):
         if self.body:
             self.body.validate()
+        if self.concurrency:
+            self.concurrency.validate()
         if self.function_name:
             self.function_name.validate()
         if self.invocation_type:
             self.invocation_type.validate()
         if self.qualifier:
             self.qualifier.validate()
         if self.service_name:
@@ -19859,14 +20334,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.body is not None:
             result['Body'] = self.body.to_map()
+        if self.concurrency is not None:
+            result['Concurrency'] = self.concurrency.to_map()
         if self.function_name is not None:
             result['FunctionName'] = self.function_name.to_map()
         if self.invocation_type is not None:
             result['InvocationType'] = self.invocation_type.to_map()
         if self.qualifier is not None:
             result['Qualifier'] = self.qualifier.to_map()
         if self.service_name is not None:
@@ -19874,14 +20351,17 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Body') is not None:
             temp_model = UpdateEventStreamingRequestSinkSinkFcParametersBody()
             self.body = temp_model.from_map(m['Body'])
+        if m.get('Concurrency') is not None:
+            temp_model = UpdateEventStreamingRequestSinkSinkFcParametersConcurrency()
+            self.concurrency = temp_model.from_map(m['Concurrency'])
         if m.get('FunctionName') is not None:
             temp_model = UpdateEventStreamingRequestSinkSinkFcParametersFunctionName()
             self.function_name = temp_model.from_map(m['FunctionName'])
         if m.get('InvocationType') is not None:
             temp_model = UpdateEventStreamingRequestSinkSinkFcParametersInvocationType()
             self.invocation_type = temp_model.from_map(m['InvocationType'])
         if m.get('Qualifier') is not None:
```

### Comparing `alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/PKG-INFO` & `alibabacloud_eventbridge20200401-1.0.8/alibabacloud_eventbridge20200401.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eventbridge20200401
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud eventbridge (20200401) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eventbridge20200401-1.0.7/setup.py` & `alibabacloud_eventbridge20200401-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eventbridge20200401.
 
-Created on 13/04/2023
+Created on 21/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eventbridge20200401"
 NAME = "alibabacloud_eventbridge20200401" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eventbridge (20200401) SDK Library for Python"
```

