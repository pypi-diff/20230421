# Comparing `tmp/posthoganalytics-3.0.0.tar.gz` & `tmp/posthoganalytics-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posthoganalytics-3.0.0.tar", last modified: Mon Apr 17 11:08:05 2023, max compression
+gzip compressed data, was "posthoganalytics-3.0.1.tar", last modified: Fri Apr 21 12:11:14 2023, max compression
```

## Comparing `posthoganalytics-3.0.0.tar` & `posthoganalytics-3.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:05.781949 posthoganalytics-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-04-17 11:07:46.000000 posthoganalytics-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-17 11:07:46.000000 posthoganalytics-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-04-17 11:08:05.781949 posthoganalytics-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-04-17 11:07:46.000000 posthoganalytics-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:05.781949 posthoganalytics-3.0.0/posthoganalytics/
--rw-r--r--   0 runner    (1001) docker     (122)    13485 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26410 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/poller.py
--rw-r--r--   0 runner    (1001) docker     (122)     3554 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/request.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:05.781949 posthoganalytics-3.0.0/posthoganalytics/sentry/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/sentry/django.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/sentry/posthog_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:05.781949 posthoganalytics-3.0.0/posthoganalytics/test/
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26002 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6352 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/test/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)   127333 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/test/test_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/test/test_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/test/test_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:05.781949 posthoganalytics-3.0.0/posthoganalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      891 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-17 11:08:05.000000 posthoganalytics-3.0.0/posthoganalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-17 11:07:46.000000 posthoganalytics-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-17 11:08:05.781949 posthoganalytics-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-04-17 11:07:46.000000 posthoganalytics-3.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-04-17 11:07:46.000000 posthoganalytics-3.0.0/setup_analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:11:14.064830 posthoganalytics-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-04-21 12:10:56.000000 posthoganalytics-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-21 12:10:56.000000 posthoganalytics-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-04-21 12:11:14.064830 posthoganalytics-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-04-21 12:10:56.000000 posthoganalytics-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:11:14.060830 posthoganalytics-3.0.1/posthoganalytics/
+-rw-r--r--   0 runner    (1001) docker     (122)    13674 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26685 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/poller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3554 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/request.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:11:14.060830 posthoganalytics-3.0.1/posthoganalytics/sentry/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/sentry/django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/sentry/posthog_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:11:14.064830 posthoganalytics-3.0.1/posthoganalytics/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27017 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6352 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/test/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)   127333 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/test/test_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/test/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/test/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-21 12:11:13.000000 posthoganalytics-3.0.1/posthoganalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:11:14.060830 posthoganalytics-3.0.1/posthoganalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-04-21 12:11:14.000000 posthoganalytics-3.0.1/posthoganalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      891 2023-04-21 12:11:14.000000 posthoganalytics-3.0.1/posthoganalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 12:11:14.000000 posthoganalytics-3.0.1/posthoganalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-21 12:11:14.000000 posthoganalytics-3.0.1/posthoganalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-21 12:11:14.000000 posthoganalytics-3.0.1/posthoganalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-21 12:10:56.000000 posthoganalytics-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-21 12:11:14.064830 posthoganalytics-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-04-21 12:10:56.000000 posthoganalytics-3.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-04-21 12:10:56.000000 posthoganalytics-3.0.1/setup_analytics.py
```

### Comparing `posthoganalytics-3.0.0/LICENSE` & `posthoganalytics-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/PKG-INFO` & `posthoganalytics-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posthoganalytics
-Version: 3.0.0
+Version: 3.0.1
 Summary: Integrate PostHog into any python application.
 Home-page: https://github.com/posthog/posthog-python
 Author: Posthog
 Author-email: hey@posthog.com
 Maintainer: PostHog
 Maintainer-email: hey@posthog.com
 License: MIT License
```

### Comparing `posthoganalytics-3.0.0/README.md` & `posthoganalytics-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/__init__.py` & `posthoganalytics-3.0.1/posthoganalytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,19 @@
         person_properties=person_properties,
         group_properties=group_properties,
         only_evaluate_locally=only_evaluate_locally,
         disable_geoip=disable_geoip,
     )
 
 
+def feature_flag_definitions():
+    """Returns loaded feature flags, if any. Helpful for debugging what flag information you have loaded."""
+    return _proxy("feature_flag_definitions")
+
+
 def page(*args, **kwargs):
     """Send a page call."""
     _proxy("page", *args, **kwargs)
 
 
 def screen(*args, **kwargs):
     """Send a screen call."""
```

### Comparing `posthoganalytics-3.0.0/posthoganalytics/client.py` & `posthoganalytics-3.0.1/posthoganalytics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,14 +531,17 @@
         send_feature_flag_events=True,
         disable_geoip=None,
     ):
         require("key", key, string_types)
         require("distinct_id", distinct_id, ID_TYPES)
         require("groups", groups, dict)
 
+        if self.disabled:
+            return None
+
         if self.feature_flags is None and self.personal_api_key:
             self.load_feature_flags()
         response = None
 
         # If loading in previous line failed
         if self.feature_flags:
             for flag in self.feature_flags:
@@ -604,14 +607,17 @@
         groups={},
         person_properties={},
         group_properties={},
         only_evaluate_locally=False,
         send_feature_flag_events=True,
         disable_geoip=None,
     ):
+        if self.disabled:
+            return None
+
         if match_value is None:
             match_value = self.get_feature_flag(
                 key,
                 distinct_id,
                 groups=groups,
                 person_properties=person_properties,
                 group_properties=group_properties,
@@ -671,14 +677,17 @@
         *,
         groups={},
         person_properties={},
         group_properties={},
         only_evaluate_locally=False,
         disable_geoip=None,
     ):
+        if self.disabled:
+            return {"featureFlags": None, "featureFlagPayloads": None}
+
         flags, payloads, fallback_to_decide = self._get_all_flags_and_payloads_locally(
             distinct_id, groups=groups, person_properties=person_properties, group_properties=group_properties
         )
         response = {"featureFlags": flags, "featureFlagPayloads": payloads}
 
         if fallback_to_decide and not only_evaluate_locally:
             try:
@@ -726,14 +735,17 @@
                     self.log.exception(f"[FEATURE FLAGS] Error while computing variant and payload: {e}")
                     fallback_to_decide = True
         else:
             fallback_to_decide = True
 
         return flags, payloads, fallback_to_decide
 
+    def feature_flag_definitions(self):
+        return self.feature_flags
+
 
 def require(name, field, data_type):
     """Require that the named `field` has the right `data_type`"""
     if not isinstance(field, data_type):
         msg = "{0} must have {1}, got: {2}".format(name, data_type, field)
         raise AssertionError(msg)
```

### Comparing `posthoganalytics-3.0.0/posthoganalytics/consumer.py` & `posthoganalytics-3.0.1/posthoganalytics/consumer.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/feature_flags.py` & `posthoganalytics-3.0.1/posthoganalytics/feature_flags.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/poller.py` & `posthoganalytics-3.0.1/posthoganalytics/poller.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/request.py` & `posthoganalytics-3.0.1/posthoganalytics/request.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/sentry/django.py` & `posthoganalytics-3.0.1/posthoganalytics/sentry/django.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/sentry/posthog_integration.py` & `posthoganalytics-3.0.1/posthoganalytics/sentry/posthog_integration.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/test/test_client.py` & `posthoganalytics-3.0.1/posthoganalytics/test/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,14 +533,41 @@
         success, msg = client.capture("distinct_id", "python test event")
         client.flush()
         self.assertFalse(success)
         self.assertFalse(self.failed)
 
         self.assertEqual(msg, "disabled")
 
+    @mock.patch("posthog.client.decide")
+    def test_disabled_with_feature_flags(self, patch_decide):
+        client = Client(FAKE_TEST_API_KEY, on_error=self.set_fail, disabled=True)
+
+        response = client.get_feature_flag("beta-feature", "12345")
+        self.assertIsNone(response)
+        patch_decide.assert_not_called()
+
+        response = client.feature_enabled("beta-feature", "12345")
+        self.assertIsNone(response)
+        patch_decide.assert_not_called()
+
+        response = client.get_all_flags("12345")
+        self.assertIsNone(response)
+        patch_decide.assert_not_called()
+
+        response = client.get_feature_flag_payload("key", "12345")
+        self.assertIsNone(response)
+        patch_decide.assert_not_called()
+
+        response = client.get_all_flags_and_payloads("12345")
+        self.assertEqual(response, {"featureFlags": None, "featureFlagPayloads": None})
+        patch_decide.assert_not_called()
+
+        # no capture calls
+        self.assertTrue(client.queue.empty())
+
     def test_enabled_to_disabled(self):
         client = Client(FAKE_TEST_API_KEY, on_error=self.set_fail, disabled=False)
         success, msg = client.capture("distinct_id", "python test event")
         client.flush()
 
         self.assertTrue(success)
         self.assertFalse(self.failed)
```

### Comparing `posthoganalytics-3.0.0/posthoganalytics/test/test_consumer.py` & `posthoganalytics-3.0.1/posthoganalytics/test/test_consumer.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/test/test_feature_flags.py` & `posthoganalytics-3.0.1/posthoganalytics/test/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/test/test_module.py` & `posthoganalytics-3.0.1/posthoganalytics/test/test_module.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/test/test_request.py` & `posthoganalytics-3.0.1/posthoganalytics/test/test_request.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/test/test_utils.py` & `posthoganalytics-3.0.1/posthoganalytics/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics/utils.py` & `posthoganalytics-3.0.1/posthoganalytics/utils.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/posthoganalytics.egg-info/PKG-INFO` & `posthoganalytics-3.0.1/posthoganalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posthoganalytics
-Version: 3.0.0
+Version: 3.0.1
 Summary: Integrate PostHog into any python application.
 Home-page: https://github.com/posthog/posthog-python
 Author: Posthog
 Author-email: hey@posthog.com
 Maintainer: PostHog
 Maintainer-email: hey@posthog.com
 License: MIT License
```

### Comparing `posthoganalytics-3.0.0/posthoganalytics.egg-info/SOURCES.txt` & `posthoganalytics-3.0.1/posthoganalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/setup.py` & `posthoganalytics-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-3.0.0/setup_analytics.py` & `posthoganalytics-3.0.1/setup_analytics.py`

 * *Files identical despite different names*

