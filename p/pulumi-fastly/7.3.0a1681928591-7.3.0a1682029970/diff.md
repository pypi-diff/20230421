# Comparing `tmp/pulumi_fastly-7.3.0a1681928591.tar.gz` & `tmp/pulumi_fastly-7.3.0a1682029970.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-7.3.0a1681928591.tar", last modified: Wed Apr 19 18:45:45 2023, max compression
+gzip compressed data, was "pulumi_fastly-7.3.0a1682029970.tar", last modified: Thu Apr 20 22:37:35 2023, max compression
```

## Comparing `pulumi_fastly-7.3.0a1681928591.tar` & `pulumi_fastly-7.3.0a1682029970.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:45.924546 pulumi_fastly-7.3.0a1681928591/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-19 18:45:45.924546 pulumi_fastly-7.3.0a1681928591/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:45.924546 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   494209 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:45.924546 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)   438935 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    93253 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (123)   122715 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    32406 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:45:45.924546 pulumi_fastly-7.3.0a1681928591/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:45:45.924546 pulumi_fastly-7.3.0a1681928591/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-19 18:45:45.000000 pulumi_fastly-7.3.0a1681928591/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   504881 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)   449591 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93253 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32406 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 22:37:35.000000 pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:37:35.043764 pulumi_fastly-7.3.0a1682029970/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-20 22:37:34.000000 pulumi_fastly-7.3.0a1682029970/setup.py
```

### Comparing `pulumi_fastly-7.3.0a1681928591/PKG-INFO` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi_fastly
-Version: 7.3.0a1681928591
+Name: pulumi-fastly
+Version: 7.3.0a1682029970
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-fastly/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-fastly/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Ffastly.svg)](https://www.npmjs.com/package/@pulumi/fastly)
 [![Python version](https://badge.fury.io/py/pulumi-fastly.svg)](https://pypi.org/project/pulumi-fastly)
 [![NuGet version](https://badge.fury.io/nu/pulumi.fastly.svg)](https://badge.fury.io/nu/pulumi.fastly)
```

### Comparing `pulumi_fastly-7.3.0a1681928591/README.md` & `pulumi_fastly-7.3.0a1682029970/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/__init__.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .get_datacenters import *
+from .get_dictionaries import *
 from .get_fastly_ip_ranges import *
 from .get_services import *
 from .get_tls_activation import *
 from .get_tls_activation_ids import *
 from .get_tls_certificate import *
 from .get_tls_certificate_ids import *
 from .get_tls_configuration import *
```

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/_inputs.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,16 @@
     'ServiceVclLoggingS3Args',
     'ServiceVclLoggingScalyrArgs',
     'ServiceVclLoggingSftpArgs',
     'ServiceVclLoggingSplunkArgs',
     'ServiceVclLoggingSumologicArgs',
     'ServiceVclLoggingSyslogArgs',
     'ServiceVclProductEnablementArgs',
+    'ServiceVclRateLimiterArgs',
+    'ServiceVclRateLimiterResponseArgs',
     'ServiceVclRequestSettingArgs',
     'ServiceVclResponseObjectArgs',
     'ServiceVclSnippetArgs',
     'ServiceVclVclArgs',
     'ServiceVclWafArgs',
     'ServiceWafConfigurationRuleArgs',
     'ServiceWafConfigurationRuleExclusionArgs',
@@ -10842,14 +10844,260 @@
 
     @websockets.setter
     def websockets(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "websockets", value)
 
 
 @pulumi.input_type
+class ServiceVclRateLimiterArgs:
+    def __init__(__self__, *,
+                 action: pulumi.Input[str],
+                 client_key: pulumi.Input[str],
+                 http_methods: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 penalty_box_duration: pulumi.Input[int],
+                 rps_limit: pulumi.Input[int],
+                 window_size: pulumi.Input[int],
+                 feature_revision: Optional[pulumi.Input[int]] = None,
+                 logger_type: Optional[pulumi.Input[str]] = None,
+                 ratelimiter_id: Optional[pulumi.Input[str]] = None,
+                 response: Optional[pulumi.Input['ServiceVclRateLimiterResponseArgs']] = None,
+                 response_object_name: Optional[pulumi.Input[str]] = None,
+                 uri_dictionary_name: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] action: The action to take when a rate limiter violation is detected (one of: log*only, log*only, response_object)
+        :param pulumi.Input[str] client_key: Comma-separated list of VCL variables used to generate a counter key to identify a client
+        :param pulumi.Input[str] http_methods: Comma-separated list of HTTP methods to apply rate limiting to
+        :param pulumi.Input[str] name: A unique human readable name for the rate limiting rule
+        :param pulumi.Input[int] penalty_box_duration: Length of time in minutes that the rate limiter is in effect after the initial violation is detected
+        :param pulumi.Input[int] rps_limit: Upper limit of requests per second allowed by the rate limiter
+        :param pulumi.Input[int] window_size: Number of seconds during which the RPS limit must be exceeded in order to trigger a violation (one of: 1, 10, 60)
+        :param pulumi.Input[int] feature_revision: Revision number of the rate limiting feature implementation
+        :param pulumi.Input[str] logger_type: Name of the type of logging endpoint to be used when action is log_only (one of: azureblob, bigquery, cloudfiles, datadog, digitalocean, elasticsearch, ftp, gcs, googleanalytics, heroku, honeycomb, http, https, kafka, kinesis, logentries, loggly, logshuttle, newrelic, openstack, papertrail, pubsub, s3, scalyr, sftp, splunk, stackdriver, sumologic, syslog)
+        :param pulumi.Input[str] ratelimiter_id: Alphanumeric string identifying the rate limiter
+        :param pulumi.Input['ServiceVclRateLimiterResponseArgs'] response: Custom response to be sent when the rate limit is exceeded. Required if action is response
+        :param pulumi.Input[str] response_object_name: Name of existing response object. Required if action is response_object
+        :param pulumi.Input[str] uri_dictionary_name: The name of an Edge Dictionary containing URIs as keys. If not defined or null, all origin URIs will be rate limited
+        """
+        pulumi.set(__self__, "action", action)
+        pulumi.set(__self__, "client_key", client_key)
+        pulumi.set(__self__, "http_methods", http_methods)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "penalty_box_duration", penalty_box_duration)
+        pulumi.set(__self__, "rps_limit", rps_limit)
+        pulumi.set(__self__, "window_size", window_size)
+        if feature_revision is not None:
+            pulumi.set(__self__, "feature_revision", feature_revision)
+        if logger_type is not None:
+            pulumi.set(__self__, "logger_type", logger_type)
+        if ratelimiter_id is not None:
+            pulumi.set(__self__, "ratelimiter_id", ratelimiter_id)
+        if response is not None:
+            pulumi.set(__self__, "response", response)
+        if response_object_name is not None:
+            pulumi.set(__self__, "response_object_name", response_object_name)
+        if uri_dictionary_name is not None:
+            pulumi.set(__self__, "uri_dictionary_name", uri_dictionary_name)
+
+    @property
+    @pulumi.getter
+    def action(self) -> pulumi.Input[str]:
+        """
+        The action to take when a rate limiter violation is detected (one of: log*only, log*only, response_object)
+        """
+        return pulumi.get(self, "action")
+
+    @action.setter
+    def action(self, value: pulumi.Input[str]):
+        pulumi.set(self, "action", value)
+
+    @property
+    @pulumi.getter(name="clientKey")
+    def client_key(self) -> pulumi.Input[str]:
+        """
+        Comma-separated list of VCL variables used to generate a counter key to identify a client
+        """
+        return pulumi.get(self, "client_key")
+
+    @client_key.setter
+    def client_key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "client_key", value)
+
+    @property
+    @pulumi.getter(name="httpMethods")
+    def http_methods(self) -> pulumi.Input[str]:
+        """
+        Comma-separated list of HTTP methods to apply rate limiting to
+        """
+        return pulumi.get(self, "http_methods")
+
+    @http_methods.setter
+    def http_methods(self, value: pulumi.Input[str]):
+        pulumi.set(self, "http_methods", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        A unique human readable name for the rate limiting rule
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="penaltyBoxDuration")
+    def penalty_box_duration(self) -> pulumi.Input[int]:
+        """
+        Length of time in minutes that the rate limiter is in effect after the initial violation is detected
+        """
+        return pulumi.get(self, "penalty_box_duration")
+
+    @penalty_box_duration.setter
+    def penalty_box_duration(self, value: pulumi.Input[int]):
+        pulumi.set(self, "penalty_box_duration", value)
+
+    @property
+    @pulumi.getter(name="rpsLimit")
+    def rps_limit(self) -> pulumi.Input[int]:
+        """
+        Upper limit of requests per second allowed by the rate limiter
+        """
+        return pulumi.get(self, "rps_limit")
+
+    @rps_limit.setter
+    def rps_limit(self, value: pulumi.Input[int]):
+        pulumi.set(self, "rps_limit", value)
+
+    @property
+    @pulumi.getter(name="windowSize")
+    def window_size(self) -> pulumi.Input[int]:
+        """
+        Number of seconds during which the RPS limit must be exceeded in order to trigger a violation (one of: 1, 10, 60)
+        """
+        return pulumi.get(self, "window_size")
+
+    @window_size.setter
+    def window_size(self, value: pulumi.Input[int]):
+        pulumi.set(self, "window_size", value)
+
+    @property
+    @pulumi.getter(name="featureRevision")
+    def feature_revision(self) -> Optional[pulumi.Input[int]]:
+        """
+        Revision number of the rate limiting feature implementation
+        """
+        return pulumi.get(self, "feature_revision")
+
+    @feature_revision.setter
+    def feature_revision(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "feature_revision", value)
+
+    @property
+    @pulumi.getter(name="loggerType")
+    def logger_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the type of logging endpoint to be used when action is log_only (one of: azureblob, bigquery, cloudfiles, datadog, digitalocean, elasticsearch, ftp, gcs, googleanalytics, heroku, honeycomb, http, https, kafka, kinesis, logentries, loggly, logshuttle, newrelic, openstack, papertrail, pubsub, s3, scalyr, sftp, splunk, stackdriver, sumologic, syslog)
+        """
+        return pulumi.get(self, "logger_type")
+
+    @logger_type.setter
+    def logger_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "logger_type", value)
+
+    @property
+    @pulumi.getter(name="ratelimiterId")
+    def ratelimiter_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Alphanumeric string identifying the rate limiter
+        """
+        return pulumi.get(self, "ratelimiter_id")
+
+    @ratelimiter_id.setter
+    def ratelimiter_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ratelimiter_id", value)
+
+    @property
+    @pulumi.getter
+    def response(self) -> Optional[pulumi.Input['ServiceVclRateLimiterResponseArgs']]:
+        """
+        Custom response to be sent when the rate limit is exceeded. Required if action is response
+        """
+        return pulumi.get(self, "response")
+
+    @response.setter
+    def response(self, value: Optional[pulumi.Input['ServiceVclRateLimiterResponseArgs']]):
+        pulumi.set(self, "response", value)
+
+    @property
+    @pulumi.getter(name="responseObjectName")
+    def response_object_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of existing response object. Required if action is response_object
+        """
+        return pulumi.get(self, "response_object_name")
+
+    @response_object_name.setter
+    def response_object_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "response_object_name", value)
+
+    @property
+    @pulumi.getter(name="uriDictionaryName")
+    def uri_dictionary_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The name of an Edge Dictionary containing URIs as keys. If not defined or null, all origin URIs will be rate limited
+        """
+        return pulumi.get(self, "uri_dictionary_name")
+
+    @uri_dictionary_name.setter
+    def uri_dictionary_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "uri_dictionary_name", value)
+
+
+@pulumi.input_type
+class ServiceVclRateLimiterResponseArgs:
+    def __init__(__self__, *,
+                 content: pulumi.Input[str],
+                 content_type: pulumi.Input[str],
+                 status: pulumi.Input[int]):
+        pulumi.set(__self__, "content", content)
+        pulumi.set(__self__, "content_type", content_type)
+        pulumi.set(__self__, "status", status)
+
+    @property
+    @pulumi.getter
+    def content(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "content")
+
+    @content.setter
+    def content(self, value: pulumi.Input[str]):
+        pulumi.set(self, "content", value)
+
+    @property
+    @pulumi.getter(name="contentType")
+    def content_type(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "content_type")
+
+    @content_type.setter
+    def content_type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "content_type", value)
+
+    @property
+    @pulumi.getter
+    def status(self) -> pulumi.Input[int]:
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: pulumi.Input[int]):
+        pulumi.set(self, "status", value)
+
+
+@pulumi.input_type
 class ServiceVclRequestSettingArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  action: Optional[pulumi.Input[str]] = None,
                  bypass_busy_wait: Optional[pulumi.Input[bool]] = None,
                  default_host: Optional[pulumi.Input[str]] = None,
                  force_miss: Optional[pulumi.Input[bool]] = None,
```

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/_utilities.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/config/vars.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_services.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example_tls_configuration_ids = fastly.get_tls_configuration_ids()
-    example_tls_activation = fastly.TlsActivation("exampleTlsActivation", configuration_id=data["fastly_tls_configuration"]["example"]["ids"])
+    example_tls_activation = fastly.TlsActivation("exampleTlsActivation", configuration_id=example_tls_configuration_ids.ids[0])
     # ...
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsConfigurationIds:getTlsConfigurationIds', __args__, opts=opts, typ=GetTlsConfigurationIdsResult).value
```

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/outputs.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
 
 __all__ = [
     'ServiceACLEntriesEntry',
     'ServiceComputeBackend',
     'ServiceComputeDictionary',
     'ServiceComputeDomain',
     'ServiceComputeLoggingBigquery',
@@ -76,24 +77,27 @@
     'ServiceVclLoggingS3',
     'ServiceVclLoggingScalyr',
     'ServiceVclLoggingSftp',
     'ServiceVclLoggingSplunk',
     'ServiceVclLoggingSumologic',
     'ServiceVclLoggingSyslog',
     'ServiceVclProductEnablement',
+    'ServiceVclRateLimiter',
+    'ServiceVclRateLimiterResponse',
     'ServiceVclRequestSetting',
     'ServiceVclResponseObject',
     'ServiceVclSnippet',
     'ServiceVclVcl',
     'ServiceVclWaf',
     'ServiceWafConfigurationRule',
     'ServiceWafConfigurationRuleExclusion',
     'TlsSubscriptionManagedDnsChallenge',
     'TlsSubscriptionManagedHttpChallenge',
     'GetDatacentersPopResult',
+    'GetDictionariesDictionaryResult',
     'GetServicesDetailResult',
     'GetTlsConfigurationDnsRecordResult',
     'GetWafRulesRuleResult',
 ]
 
 @pulumi.output_type
 class ServiceACLEntriesEntry(dict):
@@ -9730,14 +9734,248 @@
         """
         Enable WebSockets support
         """
         return pulumi.get(self, "websockets")
 
 
 @pulumi.output_type
+class ServiceVclRateLimiter(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clientKey":
+            suggest = "client_key"
+        elif key == "httpMethods":
+            suggest = "http_methods"
+        elif key == "penaltyBoxDuration":
+            suggest = "penalty_box_duration"
+        elif key == "rpsLimit":
+            suggest = "rps_limit"
+        elif key == "windowSize":
+            suggest = "window_size"
+        elif key == "featureRevision":
+            suggest = "feature_revision"
+        elif key == "loggerType":
+            suggest = "logger_type"
+        elif key == "ratelimiterId":
+            suggest = "ratelimiter_id"
+        elif key == "responseObjectName":
+            suggest = "response_object_name"
+        elif key == "uriDictionaryName":
+            suggest = "uri_dictionary_name"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ServiceVclRateLimiter. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ServiceVclRateLimiter.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ServiceVclRateLimiter.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 action: str,
+                 client_key: str,
+                 http_methods: str,
+                 name: str,
+                 penalty_box_duration: int,
+                 rps_limit: int,
+                 window_size: int,
+                 feature_revision: Optional[int] = None,
+                 logger_type: Optional[str] = None,
+                 ratelimiter_id: Optional[str] = None,
+                 response: Optional['outputs.ServiceVclRateLimiterResponse'] = None,
+                 response_object_name: Optional[str] = None,
+                 uri_dictionary_name: Optional[str] = None):
+        """
+        :param str action: The action to take when a rate limiter violation is detected (one of: log*only, log*only, response_object)
+        :param str client_key: Comma-separated list of VCL variables used to generate a counter key to identify a client
+        :param str http_methods: Comma-separated list of HTTP methods to apply rate limiting to
+        :param str name: A unique human readable name for the rate limiting rule
+        :param int penalty_box_duration: Length of time in minutes that the rate limiter is in effect after the initial violation is detected
+        :param int rps_limit: Upper limit of requests per second allowed by the rate limiter
+        :param int window_size: Number of seconds during which the RPS limit must be exceeded in order to trigger a violation (one of: 1, 10, 60)
+        :param int feature_revision: Revision number of the rate limiting feature implementation
+        :param str logger_type: Name of the type of logging endpoint to be used when action is log_only (one of: azureblob, bigquery, cloudfiles, datadog, digitalocean, elasticsearch, ftp, gcs, googleanalytics, heroku, honeycomb, http, https, kafka, kinesis, logentries, loggly, logshuttle, newrelic, openstack, papertrail, pubsub, s3, scalyr, sftp, splunk, stackdriver, sumologic, syslog)
+        :param str ratelimiter_id: Alphanumeric string identifying the rate limiter
+        :param 'ServiceVclRateLimiterResponseArgs' response: Custom response to be sent when the rate limit is exceeded. Required if action is response
+        :param str response_object_name: Name of existing response object. Required if action is response_object
+        :param str uri_dictionary_name: The name of an Edge Dictionary containing URIs as keys. If not defined or null, all origin URIs will be rate limited
+        """
+        pulumi.set(__self__, "action", action)
+        pulumi.set(__self__, "client_key", client_key)
+        pulumi.set(__self__, "http_methods", http_methods)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "penalty_box_duration", penalty_box_duration)
+        pulumi.set(__self__, "rps_limit", rps_limit)
+        pulumi.set(__self__, "window_size", window_size)
+        if feature_revision is not None:
+            pulumi.set(__self__, "feature_revision", feature_revision)
+        if logger_type is not None:
+            pulumi.set(__self__, "logger_type", logger_type)
+        if ratelimiter_id is not None:
+            pulumi.set(__self__, "ratelimiter_id", ratelimiter_id)
+        if response is not None:
+            pulumi.set(__self__, "response", response)
+        if response_object_name is not None:
+            pulumi.set(__self__, "response_object_name", response_object_name)
+        if uri_dictionary_name is not None:
+            pulumi.set(__self__, "uri_dictionary_name", uri_dictionary_name)
+
+    @property
+    @pulumi.getter
+    def action(self) -> str:
+        """
+        The action to take when a rate limiter violation is detected (one of: log*only, log*only, response_object)
+        """
+        return pulumi.get(self, "action")
+
+    @property
+    @pulumi.getter(name="clientKey")
+    def client_key(self) -> str:
+        """
+        Comma-separated list of VCL variables used to generate a counter key to identify a client
+        """
+        return pulumi.get(self, "client_key")
+
+    @property
+    @pulumi.getter(name="httpMethods")
+    def http_methods(self) -> str:
+        """
+        Comma-separated list of HTTP methods to apply rate limiting to
+        """
+        return pulumi.get(self, "http_methods")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        A unique human readable name for the rate limiting rule
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="penaltyBoxDuration")
+    def penalty_box_duration(self) -> int:
+        """
+        Length of time in minutes that the rate limiter is in effect after the initial violation is detected
+        """
+        return pulumi.get(self, "penalty_box_duration")
+
+    @property
+    @pulumi.getter(name="rpsLimit")
+    def rps_limit(self) -> int:
+        """
+        Upper limit of requests per second allowed by the rate limiter
+        """
+        return pulumi.get(self, "rps_limit")
+
+    @property
+    @pulumi.getter(name="windowSize")
+    def window_size(self) -> int:
+        """
+        Number of seconds during which the RPS limit must be exceeded in order to trigger a violation (one of: 1, 10, 60)
+        """
+        return pulumi.get(self, "window_size")
+
+    @property
+    @pulumi.getter(name="featureRevision")
+    def feature_revision(self) -> Optional[int]:
+        """
+        Revision number of the rate limiting feature implementation
+        """
+        return pulumi.get(self, "feature_revision")
+
+    @property
+    @pulumi.getter(name="loggerType")
+    def logger_type(self) -> Optional[str]:
+        """
+        Name of the type of logging endpoint to be used when action is log_only (one of: azureblob, bigquery, cloudfiles, datadog, digitalocean, elasticsearch, ftp, gcs, googleanalytics, heroku, honeycomb, http, https, kafka, kinesis, logentries, loggly, logshuttle, newrelic, openstack, papertrail, pubsub, s3, scalyr, sftp, splunk, stackdriver, sumologic, syslog)
+        """
+        return pulumi.get(self, "logger_type")
+
+    @property
+    @pulumi.getter(name="ratelimiterId")
+    def ratelimiter_id(self) -> Optional[str]:
+        """
+        Alphanumeric string identifying the rate limiter
+        """
+        return pulumi.get(self, "ratelimiter_id")
+
+    @property
+    @pulumi.getter
+    def response(self) -> Optional['outputs.ServiceVclRateLimiterResponse']:
+        """
+        Custom response to be sent when the rate limit is exceeded. Required if action is response
+        """
+        return pulumi.get(self, "response")
+
+    @property
+    @pulumi.getter(name="responseObjectName")
+    def response_object_name(self) -> Optional[str]:
+        """
+        Name of existing response object. Required if action is response_object
+        """
+        return pulumi.get(self, "response_object_name")
+
+    @property
+    @pulumi.getter(name="uriDictionaryName")
+    def uri_dictionary_name(self) -> Optional[str]:
+        """
+        The name of an Edge Dictionary containing URIs as keys. If not defined or null, all origin URIs will be rate limited
+        """
+        return pulumi.get(self, "uri_dictionary_name")
+
+
+@pulumi.output_type
+class ServiceVclRateLimiterResponse(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "contentType":
+            suggest = "content_type"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ServiceVclRateLimiterResponse. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ServiceVclRateLimiterResponse.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ServiceVclRateLimiterResponse.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 content: str,
+                 content_type: str,
+                 status: int):
+        pulumi.set(__self__, "content", content)
+        pulumi.set(__self__, "content_type", content_type)
+        pulumi.set(__self__, "status", status)
+
+    @property
+    @pulumi.getter
+    def content(self) -> str:
+        return pulumi.get(self, "content")
+
+    @property
+    @pulumi.getter(name="contentType")
+    def content_type(self) -> str:
+        return pulumi.get(self, "content_type")
+
+    @property
+    @pulumi.getter
+    def status(self) -> int:
+        return pulumi.get(self, "status")
+
+
+@pulumi.output_type
 class ServiceVclRequestSetting(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bypassBusyWait":
             suggest = "bypass_busy_wait"
         elif key == "defaultHost":
@@ -10494,14 +10732,46 @@
     @property
     @pulumi.getter
     def shield(self) -> str:
         return pulumi.get(self, "shield")
 
 
 @pulumi.output_type
+class GetDictionariesDictionaryResult(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 name: str,
+                 write_only: bool):
+        """
+        :param str id: The ID of this resource.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "write_only", write_only)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The ID of this resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="writeOnly")
+    def write_only(self) -> bool:
+        return pulumi.get(self, "write_only")
+
+
+@pulumi.output_type
 class GetServicesDetailResult(dict):
     def __init__(__self__, *,
                  comment: str,
                  created_at: str,
                  customer_id: str,
                  id: str,
                  name: str,
```

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/provider.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_authorization.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_compute.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_vcl.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_vcl.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
                  logging_scalyrs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingScalyrArgs']]]] = None,
                  logging_sftps: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingSftpArgs']]]] = None,
                  logging_splunks: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingSplunkArgs']]]] = None,
                  logging_sumologics: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingSumologicArgs']]]] = None,
                  logging_syslogs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingSyslogArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  product_enablement: Optional[pulumi.Input['ServiceVclProductEnablementArgs']] = None,
+                 rate_limiters: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRateLimiterArgs']]]] = None,
                  request_settings: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRequestSettingArgs']]]] = None,
                  response_objects: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclResponseObjectArgs']]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  snippets: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclSnippetArgs']]]] = None,
                  stale_if_error: Optional[pulumi.Input[bool]] = None,
                  stale_if_error_ttl: Optional[pulumi.Input[int]] = None,
                  vcls: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclVclArgs']]]] = None,
@@ -172,14 +173,16 @@
             pulumi.set(__self__, "logging_sumologics", logging_sumologics)
         if logging_syslogs is not None:
             pulumi.set(__self__, "logging_syslogs", logging_syslogs)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if product_enablement is not None:
             pulumi.set(__self__, "product_enablement", product_enablement)
+        if rate_limiters is not None:
+            pulumi.set(__self__, "rate_limiters", rate_limiters)
         if request_settings is not None:
             pulumi.set(__self__, "request_settings", request_settings)
         if response_objects is not None:
             pulumi.set(__self__, "response_objects", response_objects)
         if reuse is not None:
             pulumi.set(__self__, "reuse", reuse)
         if snippets is not None:
@@ -621,14 +624,23 @@
         return pulumi.get(self, "product_enablement")
 
     @product_enablement.setter
     def product_enablement(self, value: Optional[pulumi.Input['ServiceVclProductEnablementArgs']]):
         pulumi.set(self, "product_enablement", value)
 
     @property
+    @pulumi.getter(name="rateLimiters")
+    def rate_limiters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRateLimiterArgs']]]]:
+        return pulumi.get(self, "rate_limiters")
+
+    @rate_limiters.setter
+    def rate_limiters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRateLimiterArgs']]]]):
+        pulumi.set(self, "rate_limiters", value)
+
+    @property
     @pulumi.getter(name="requestSettings")
     def request_settings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRequestSettingArgs']]]]:
         return pulumi.get(self, "request_settings")
 
     @request_settings.setter
     def request_settings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRequestSettingArgs']]]]):
         pulumi.set(self, "request_settings", value)
@@ -768,14 +780,15 @@
                  logging_scalyrs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingScalyrArgs']]]] = None,
                  logging_sftps: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingSftpArgs']]]] = None,
                  logging_splunks: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingSplunkArgs']]]] = None,
                  logging_sumologics: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingSumologicArgs']]]] = None,
                  logging_syslogs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingSyslogArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  product_enablement: Optional[pulumi.Input['ServiceVclProductEnablementArgs']] = None,
+                 rate_limiters: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRateLimiterArgs']]]] = None,
                  request_settings: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRequestSettingArgs']]]] = None,
                  response_objects: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclResponseObjectArgs']]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  snippets: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclSnippetArgs']]]] = None,
                  stale_if_error: Optional[pulumi.Input[bool]] = None,
                  stale_if_error_ttl: Optional[pulumi.Input[int]] = None,
                  vcls: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclVclArgs']]]] = None,
@@ -898,14 +911,16 @@
             pulumi.set(__self__, "logging_sumologics", logging_sumologics)
         if logging_syslogs is not None:
             pulumi.set(__self__, "logging_syslogs", logging_syslogs)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if product_enablement is not None:
             pulumi.set(__self__, "product_enablement", product_enablement)
+        if rate_limiters is not None:
+            pulumi.set(__self__, "rate_limiters", rate_limiters)
         if request_settings is not None:
             pulumi.set(__self__, "request_settings", request_settings)
         if response_objects is not None:
             pulumi.set(__self__, "response_objects", response_objects)
         if reuse is not None:
             pulumi.set(__self__, "reuse", reuse)
         if snippets is not None:
@@ -1397,14 +1412,23 @@
         return pulumi.get(self, "product_enablement")
 
     @product_enablement.setter
     def product_enablement(self, value: Optional[pulumi.Input['ServiceVclProductEnablementArgs']]):
         pulumi.set(self, "product_enablement", value)
 
     @property
+    @pulumi.getter(name="rateLimiters")
+    def rate_limiters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRateLimiterArgs']]]]:
+        return pulumi.get(self, "rate_limiters")
+
+    @rate_limiters.setter
+    def rate_limiters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRateLimiterArgs']]]]):
+        pulumi.set(self, "rate_limiters", value)
+
+    @property
     @pulumi.getter(name="requestSettings")
     def request_settings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRequestSettingArgs']]]]:
         return pulumi.get(self, "request_settings")
 
     @request_settings.setter
     def request_settings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRequestSettingArgs']]]]):
         pulumi.set(self, "request_settings", value)
@@ -1542,14 +1566,15 @@
                  logging_scalyrs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingScalyrArgs']]]]] = None,
                  logging_sftps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSftpArgs']]]]] = None,
                  logging_splunks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSplunkArgs']]]]] = None,
                  logging_sumologics: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSumologicArgs']]]]] = None,
                  logging_syslogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSyslogArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  product_enablement: Optional[pulumi.Input[pulumi.InputType['ServiceVclProductEnablementArgs']]] = None,
+                 rate_limiters: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclRateLimiterArgs']]]]] = None,
                  request_settings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclRequestSettingArgs']]]]] = None,
                  response_objects: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclResponseObjectArgs']]]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  snippets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclSnippetArgs']]]]] = None,
                  stale_if_error: Optional[pulumi.Input[bool]] = None,
                  stale_if_error_ttl: Optional[pulumi.Input[int]] = None,
                  vcls: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclVclArgs']]]]] = None,
@@ -1681,14 +1706,15 @@
                  logging_scalyrs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingScalyrArgs']]]]] = None,
                  logging_sftps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSftpArgs']]]]] = None,
                  logging_splunks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSplunkArgs']]]]] = None,
                  logging_sumologics: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSumologicArgs']]]]] = None,
                  logging_syslogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSyslogArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  product_enablement: Optional[pulumi.Input[pulumi.InputType['ServiceVclProductEnablementArgs']]] = None,
+                 rate_limiters: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclRateLimiterArgs']]]]] = None,
                  request_settings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclRequestSettingArgs']]]]] = None,
                  response_objects: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclResponseObjectArgs']]]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  snippets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclSnippetArgs']]]]] = None,
                  stale_if_error: Optional[pulumi.Input[bool]] = None,
                  stale_if_error_ttl: Optional[pulumi.Input[int]] = None,
                  vcls: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclVclArgs']]]]] = None,
@@ -1746,14 +1772,15 @@
             __props__.__dict__["logging_scalyrs"] = logging_scalyrs
             __props__.__dict__["logging_sftps"] = logging_sftps
             __props__.__dict__["logging_splunks"] = logging_splunks
             __props__.__dict__["logging_sumologics"] = logging_sumologics
             __props__.__dict__["logging_syslogs"] = logging_syslogs
             __props__.__dict__["name"] = name
             __props__.__dict__["product_enablement"] = product_enablement
+            __props__.__dict__["rate_limiters"] = rate_limiters
             __props__.__dict__["request_settings"] = request_settings
             __props__.__dict__["response_objects"] = response_objects
             __props__.__dict__["reuse"] = reuse
             __props__.__dict__["snippets"] = snippets
             __props__.__dict__["stale_if_error"] = stale_if_error
             __props__.__dict__["stale_if_error_ttl"] = stale_if_error_ttl
             __props__.__dict__["vcls"] = vcls
@@ -1818,14 +1845,15 @@
             logging_scalyrs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingScalyrArgs']]]]] = None,
             logging_sftps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSftpArgs']]]]] = None,
             logging_splunks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSplunkArgs']]]]] = None,
             logging_sumologics: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSumologicArgs']]]]] = None,
             logging_syslogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclLoggingSyslogArgs']]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             product_enablement: Optional[pulumi.Input[pulumi.InputType['ServiceVclProductEnablementArgs']]] = None,
+            rate_limiters: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclRateLimiterArgs']]]]] = None,
             request_settings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclRequestSettingArgs']]]]] = None,
             response_objects: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclResponseObjectArgs']]]]] = None,
             reuse: Optional[pulumi.Input[bool]] = None,
             snippets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclSnippetArgs']]]]] = None,
             stale_if_error: Optional[pulumi.Input[bool]] = None,
             stale_if_error_ttl: Optional[pulumi.Input[int]] = None,
             vcls: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclVclArgs']]]]] = None,
@@ -1908,14 +1936,15 @@
         __props__.__dict__["logging_scalyrs"] = logging_scalyrs
         __props__.__dict__["logging_sftps"] = logging_sftps
         __props__.__dict__["logging_splunks"] = logging_splunks
         __props__.__dict__["logging_sumologics"] = logging_sumologics
         __props__.__dict__["logging_syslogs"] = logging_syslogs
         __props__.__dict__["name"] = name
         __props__.__dict__["product_enablement"] = product_enablement
+        __props__.__dict__["rate_limiters"] = rate_limiters
         __props__.__dict__["request_settings"] = request_settings
         __props__.__dict__["response_objects"] = response_objects
         __props__.__dict__["reuse"] = reuse
         __props__.__dict__["snippets"] = snippets
         __props__.__dict__["stale_if_error"] = stale_if_error
         __props__.__dict__["stale_if_error_ttl"] = stale_if_error_ttl
         __props__.__dict__["vcls"] = vcls
@@ -2203,14 +2232,19 @@
 
     @property
     @pulumi.getter(name="productEnablement")
     def product_enablement(self) -> pulumi.Output[Optional['outputs.ServiceVclProductEnablement']]:
         return pulumi.get(self, "product_enablement")
 
     @property
+    @pulumi.getter(name="rateLimiters")
+    def rate_limiters(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclRateLimiter']]]:
+        return pulumi.get(self, "rate_limiters")
+
+    @property
     @pulumi.getter(name="requestSettings")
     def request_settings(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclRequestSetting']]]:
         return pulumi.get(self, "request_settings")
 
     @property
     @pulumi.getter(name="responseObjects")
     def response_objects(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclResponseObject']]]:
```

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_activation.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly/user.py` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-7.3.0a1682029970/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi-fastly
-Version: 7.3.0a1681928591
+Name: pulumi_fastly
+Version: 7.3.0a1682029970
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-fastly/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-fastly/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Ffastly.svg)](https://www.npmjs.com/package/@pulumi/fastly)
 [![Python version](https://badge.fury.io/py/pulumi-fastly.svg)](https://pypi.org/project/pulumi-fastly)
 [![NuGet version](https://badge.fury.io/nu/pulumi.fastly.svg)](https://badge.fury.io/nu/pulumi.fastly)
```

### Comparing `pulumi_fastly-7.3.0a1681928591/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-7.3.0a1682029970/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 pulumi_fastly/__init__.py
 pulumi_fastly/_inputs.py
 pulumi_fastly/_utilities.py
 pulumi_fastly/get_datacenters.py
+pulumi_fastly/get_dictionaries.py
 pulumi_fastly/get_fastly_ip_ranges.py
 pulumi_fastly/get_services.py
 pulumi_fastly/get_tls_activation.py
 pulumi_fastly/get_tls_activation_ids.py
 pulumi_fastly/get_tls_certificate.py
 pulumi_fastly/get_tls_certificate_ids.py
 pulumi_fastly/get_tls_configuration.py
```

### Comparing `pulumi_fastly-7.3.0a1681928591/setup.py` & `pulumi_fastly-7.3.0a1682029970/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "7.3.0a1681928591"
-PLUGIN_VERSION = "7.3.0-alpha.1681928591+3dd30944"
+VERSION = "7.3.0a1682029970"
+PLUGIN_VERSION = "7.3.0-alpha.1682029970+a58f0717"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'fastly', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "fastly Pulumi Package - Development Version"
 
 
 setup(name='pulumi_fastly',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing fastly cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

