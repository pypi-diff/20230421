# Comparing `tmp/posthog-3.0.0.tar.gz` & `tmp/posthog-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posthog-3.0.0.tar", last modified: Mon Apr 17 11:08:00 2023, max compression
+gzip compressed data, was "posthog-3.0.1.tar", last modified: Fri Apr 21 12:11:08 2023, max compression
```

## Comparing `posthog-3.0.0.tar` & `posthog-3.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:00.917886 posthog-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-04-17 11:07:46.000000 posthog-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-17 11:07:46.000000 posthog-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-17 11:08:00.917886 posthog-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-04-17 11:07:46.000000 posthog-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:00.913886 posthog-3.0.0/posthog/
--rw-r--r--   0 runner    (1001) docker     (122)    13467 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26356 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/poller.py
--rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/request.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:00.913886 posthog-3.0.0/posthog/sentry/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/sentry/django.py
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/sentry/posthog_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:00.917886 posthog-3.0.0/posthog/test/
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25975 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)   127297 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-17 11:07:46.000000 posthog-3.0.0/posthog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:08:00.913886 posthog-3.0.0/posthog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-17 11:08:00.000000 posthog-3.0.0/posthog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-17 11:08:00.000000 posthog-3.0.0/posthog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 11:08:00.000000 posthog-3.0.0/posthog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-04-17 11:08:00.000000 posthog-3.0.0/posthog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-17 11:08:00.000000 posthog-3.0.0/posthog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-17 11:07:46.000000 posthog-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-17 11:08:00.917886 posthog-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-04-17 11:07:46.000000 posthog-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:11:08.700761 posthog-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-04-21 12:10:56.000000 posthog-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-21 12:10:56.000000 posthog-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-21 12:11:08.700761 posthog-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-04-21 12:10:56.000000 posthog-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:11:08.696761 posthog-3.0.1/posthog/
+-rw-r--r--   0 runner    (1001) docker     (122)    13656 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26631 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/poller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/request.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:11:08.696761 posthog-3.0.1/posthog/sentry/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/sentry/django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/sentry/posthog_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:11:08.700761 posthog-3.0.1/posthog/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26990 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/test/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)   127297 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/test/test_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/test/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/test/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-21 12:10:56.000000 posthog-3.0.1/posthog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 12:11:08.696761 posthog-3.0.1/posthog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-21 12:11:08.000000 posthog-3.0.1/posthog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-21 12:11:08.000000 posthog-3.0.1/posthog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 12:11:08.000000 posthog-3.0.1/posthog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-04-21 12:11:08.000000 posthog-3.0.1/posthog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-21 12:11:08.000000 posthog-3.0.1/posthog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-21 12:10:56.000000 posthog-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-21 12:11:08.700761 posthog-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-04-21 12:10:56.000000 posthog-3.0.1/setup.py
```

### Comparing `posthog-3.0.0/LICENSE` & `posthog-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/PKG-INFO` & `posthog-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posthog
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

### Comparing `posthog-3.0.0/README.md` & `posthog-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/__init__.py` & `posthog-3.0.1/posthog/__init__.py`

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

### Comparing `posthog-3.0.0/posthog/client.py` & `posthog-3.0.1/posthog/client.py`

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

### Comparing `posthog-3.0.0/posthog/consumer.py` & `posthog-3.0.1/posthog/consumer.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/feature_flags.py` & `posthog-3.0.1/posthog/feature_flags.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/poller.py` & `posthog-3.0.1/posthog/poller.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/request.py` & `posthog-3.0.1/posthog/request.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/sentry/django.py` & `posthog-3.0.1/posthog/sentry/django.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/sentry/posthog_integration.py` & `posthog-3.0.1/posthog/sentry/posthog_integration.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/test/test_client.py` & `posthog-3.0.1/posthog/test/test_client.py`

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

### Comparing `posthog-3.0.0/posthog/test/test_consumer.py` & `posthog-3.0.1/posthog/test/test_consumer.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/test/test_feature_flags.py` & `posthog-3.0.1/posthog/test/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/test/test_module.py` & `posthog-3.0.1/posthog/test/test_module.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/test/test_request.py` & `posthog-3.0.1/posthog/test/test_request.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/test/test_utils.py` & `posthog-3.0.1/posthog/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog/utils.py` & `posthog-3.0.1/posthog/utils.py`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/posthog.egg-info/PKG-INFO` & `posthog-3.0.1/posthog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posthog
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

### Comparing `posthog-3.0.0/posthog.egg-info/SOURCES.txt` & `posthog-3.0.1/posthog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `posthog-3.0.0/setup.py` & `posthog-3.0.1/setup.py`

 * *Files identical despite different names*

