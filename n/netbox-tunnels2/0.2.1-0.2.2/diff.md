# Comparing `tmp/netbox-tunnels2-0.2.1.tar.gz` & `tmp/netbox-tunnels2-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-tunnels2-0.2.1.tar", last modified: Wed Apr 19 17:07:46 2023, max compression
+gzip compressed data, was "netbox-tunnels2-0.2.2.tar", last modified: Fri Apr 21 16:43:28 2023, max compression
```

## Comparing `netbox-tunnels2-0.2.1.tar` & `netbox-tunnels2-0.2.2.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.586333 netbox-tunnels2-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.590333 netbox-tunnels2-0.2.1/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   221681 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/docs/img/tunnel-info.png
--rw-r--r--   0 runner    (1001) docker     (123)   150947 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/docs/img/tunnel-list.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.590333 netbox-tunnels2-0.2.1/netbox_tunnels2/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/netbox_tunnels2/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/netbox_tunnels2/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.590333 netbox-tunnels2-0.2.1/netbox_tunnels2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/netbox_tunnels2/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.590333 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-19 17:07:46.000000 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-19 17:07:46.000000 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:07:46.000000 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 17:07:46.000000 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 17:07:46.000000 netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:07:46.594333 netbox-tunnels2-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 17:07:35.000000 netbox-tunnels2-0.2.1/tests/test_netbox_tunnels_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.563734 netbox-tunnels2-0.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.567735 netbox-tunnels2-0.2.2/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   221681 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/docs/img/tunnel-info.png
+-rw-r--r--   0 runner    (1001) docker     (123)   150947 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/docs/img/tunnel-list.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.567735 netbox-tunnels2-0.2.2/netbox_tunnels2/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/netbox_tunnels2/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.567735 netbox-tunnels2-0.2.2/netbox_tunnels2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/netbox_tunnels2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/tests/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/netbox_tunnels2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:43:28.567735 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-21 16:43:28.000000 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-21 16:43:28.000000 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:43:28.000000 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 16:43:28.000000 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 16:43:28.000000 netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-21 16:43:28.571735 netbox-tunnels2-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-21 16:43:15.000000 netbox-tunnels2-0.2.2/setup.py
```

### Comparing `netbox-tunnels2-0.2.1/CONTRIBUTING.md` & `netbox-tunnels2-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/LICENSE` & `netbox-tunnels2-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/PKG-INFO` & `netbox-tunnels2-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-tunnels2
-Version: 0.2.1
+Version: 0.2.2
 Summary: Provides the ability track IP Tunnels.
 Home-page: https://github.com/robertlynch3/netbox-tunnels2
 Author: Robert Lynch
 Author-email: Robert Lynch <robertlynch3@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `netbox-tunnels2-0.2.1/README.md` & `netbox-tunnels2-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/docs/img/tunnel-info.png` & `netbox-tunnels2-0.2.2/docs/img/tunnel-info.png`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/docs/img/tunnel-list.png` & `netbox-tunnels2-0.2.2/docs/img/tunnel-list.png`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/__init__.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/api/serializers.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/api/views.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/filtersets.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/forms.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/graphql.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/migrations/0001_initial.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/models.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,17 @@
         related_name='tunnel_a_pub_address',
         verbose_name="Side A Public Address"
     )
     b_pub_address=models.ForeignKey(
         to='ipam.IPAddress',
         on_delete=models.PROTECT,
         related_name='tunnel_b_pub_address',
-        verbose_name="Side B Public Address"
+        verbose_name="Side B Public Address",
+        null=True,
+        blank=True
     )
     description = models.CharField(
         max_length=200,
         blank=True
     )
     psk = models.CharField(verbose_name="Pre-shared Key", max_length=100, blank=True)
     comments = models.TextField(blank=True)
```

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/navigation.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/tables.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html` & `netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html` & `netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html` & `netbox-tunnels2-0.2.2/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/urls.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2/views.py` & `netbox-tunnels2-0.2.2/netbox_tunnels2/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,109 +2,109 @@
 from utilities.utils import count_related
 
 from netbox.views.generic import BulkDeleteView, BulkImportView, ObjectEditView, ObjectListView, ObjectView, ObjectDeleteView
 
 from . import forms, models, tables, filtersets
 
 class TunnelView(PermissionRequiredMixin, ObjectView):
-    permission_required = "netbox_tunnels2.view_tunnels"
+    permission_required = "netbox_tunnels2.view_tunnel"
     queryset = models.Tunnel.objects.all()
 
 class ListTunnelView(PermissionRequiredMixin, ObjectListView):
     """View for listing all Tunnels."""
 
-    permission_required = "netbox_tunnels2.view_tunnels"
+    permission_required = "netbox_tunnels2.view_tunnel"
     model = models.Tunnel
     queryset = models.Tunnel.objects.all().order_by("id")
     filterset = filtersets.TunnelFilterSet
     filterset_form = forms.TunnelFilterForm
     table = tables.TunnelTable
     
 
 class EditTunnelView(PermissionRequiredMixin, ObjectEditView):
     """View for creating a new Tunnels."""
 
-    permission_required = "netbox_tunnels2.add_tunnels"
+    permission_required = "netbox_tunnels2.change_tunnel"
     model = models.Tunnel
     queryset = models.Tunnel.objects.all()
     form = forms.TunnelEditForm
     default_return_url = "plugins:netbox_tunnels2:tunnel_list"
     template_name = "netbox_tunnels2/tunnel_edit.html"
 
 class CreateTunnelView(PermissionRequiredMixin, ObjectEditView):
     """View for creating a new Tunnels."""
-    permission_required = "netbox_tunnels2.add_tunnels"
+    permission_required = "netbox_tunnels2.add_tunnel"
     model = models.Tunnel
     queryset = models.Tunnel.objects.all()
     #form = forms.TunnelAddForm
     form = forms.TunnelEditForm
     default_return_url = "plugins:netbox_tunnels2:tunnel_list"
     template_name = "netbox_tunnels2/tunnel_edit.html"
 
 class DeleteTunnelView(PermissionRequiredMixin,ObjectDeleteView):
-    permission_required = "netbox_tunnels2.delete_tunnels"
+    permission_required = "netbox_tunnels2.delete_tunnel"
     queryset = models.Tunnel.objects.all()
     default_return_url = "plugins:netbox_tunnels2:tunnel_list"
 
 class BulkDeleteTunnelView(PermissionRequiredMixin, BulkDeleteView):
     """View for deleting one or more Tunnels."""
 
-    permission_required = "netbox_tunnels2.delete_tunnels"
+    permission_required = "netbox_tunnels2.delete_tunnel"
     queryset = models.Tunnel.objects.filter()
     table = tables.TunnelTable
     default_return_url = "plugins:netbox_tunnels2:tunnel_list"
 
 
 
 #
 # Tunnel Type
 #
 
 class TunnelTypeView(PermissionRequiredMixin, ObjectView):
-    permission_required = "netbox_tunnels2.view_type_tunnels"
+    permission_required = "netbox_tunnels2.view_tunneltype"
     queryset = models.TunnelType.objects.all()
     def get_extra_context(self, request, instance):
         table = tables.TunnelTable(instance.tunnels.all())
         table.configure(request)
         return {
             'tunnel_table': table,
         }
 
 class ListTunnelTypeView(PermissionRequiredMixin, ObjectListView):
     """View for listing all Tunnels."""
-    permission_required = "netbox_tunnels2.view_type_tunnels"
+    permission_required = "netbox_tunnels2.view_tunneltype"
     model = models.TunnelType
     queryset = models.TunnelType.objects.annotate(tunnel_count=count_related(models.Tunnel,'tunnel_type'))
     table = tables.TunnelTypeTable
     
 
 class EditTunnelTypeView(PermissionRequiredMixin, ObjectEditView):
     """View for creating a new Tunnels."""
 
-    permission_required = "netbox_tunnels2.add_tunnels"
+    permission_required = "netbox_tunnels2.change_tunneltype"
     model = models.TunnelType
     queryset = models.TunnelType.objects.all()
     form = forms.TunnelTypeEditForm
     default_return_url = "plugins:netbox_tunnels2:tunneltype_list"
 
 class CreateTunnelTypeView(PermissionRequiredMixin, ObjectEditView):
     """View for creating a new Tunnels."""
 
-    permission_required = "netbox_tunnels2.add_tunnels"
+    permission_required = "netbox_tunnels2.add_tunneltype"
     model = models.TunnelType
     queryset = models.TunnelType.objects.all()
     form = forms.TunnelTypeEditForm
     default_return_url = "plugins:netbox_tunnels2:tunneltype_list"
     
 class DeleteTunnelTypeView(PermissionRequiredMixin,ObjectDeleteView):
-    permission_required = "netbox_tunnels2.delete_tunnels"
+    permission_required = "netbox_tunnels2.delete_tunneltype"
     queryset = models.TunnelType.objects.all()
     default_return_url = "plugins:netbox_tunnels2:tunneltype_list"
 
 
 class BulkDeleteTunnelTypeView(PermissionRequiredMixin, BulkDeleteView):
     """View for deleting one or more Tunnels."""
 
-    permission_required = "netbox_tunnels2.delete_tunnels"
+    permission_required = "netbox_tunnels2.delete_tunneltype"
     queryset = models.TunnelType.objects.filter()
     table = tables.TunnelTable
     default_return_url = "plugins:netbox_tunnels2:tunneltype_list"
```

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/PKG-INFO` & `netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-tunnels2
-Version: 0.2.1
+Version: 0.2.2
 Summary: Provides the ability track IP Tunnels.
 Home-page: https://github.com/robertlynch3/netbox-tunnels2
 Author: Robert Lynch
 Author-email: Robert Lynch <robertlynch3@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `netbox-tunnels2-0.2.1/netbox_tunnels2.egg-info/SOURCES.txt` & `netbox-tunnels2-0.2.2/netbox_tunnels2.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -26,13 +26,16 @@
 netbox_tunnels2.egg-info/requires.txt
 netbox_tunnels2.egg-info/top_level.txt
 netbox_tunnels2/api/__init__.py
 netbox_tunnels2/api/serializers.py
 netbox_tunnels2/api/urls.py
 netbox_tunnels2/api/views.py
 netbox_tunnels2/migrations/0001_initial.py
+netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py
 netbox_tunnels2/migrations/__init__.py
 netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
 netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
 netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
-tests/__init__.py
-tests/test_netbox_tunnels_plugin.py
+netbox_tunnels2/tests/__init__.py
+netbox_tunnels2/tests/custom.py
+netbox_tunnels2/tests/test_api.py
+netbox_tunnels2/tests/test_models.py
```

### Comparing `netbox-tunnels2-0.2.1/pyproject.toml` & `netbox-tunnels2-0.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,43 +2,35 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-tunnels2"
-version = "0.2.1"
+version = "0.2.2"
 description = "Provides the ability track IP Tunnels."
 readme = "README.md"
 authors = [{ name = "Robert Lynch", email = "robertlynch3@users.noreply.github.com" }]
 license = { file = "LICENSE" }
 
 [project.urls]
 Homepage = "https://github.com/robertlynch3/netbox-tunnels2"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
-current_version = "0.2.1"
+current_version = "0.2.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
-    'current_version = "{version}"',
+    'current_version = "{version}"$',
+    'version = "{version}"$',
 ]
-"setup.py" = [
-    "{version}",
-    "{pep440_version}",
-]
-"README.md" = [
-    "{version}",
-    "{pep440_version}",
-]
-"netbox_tunnels2/__init__.py" = [
-    "{version}",
-    "{__version__}",
+"netbox_tunnels2/version.py" = [
+    '__version__="{version}"$',
 ]
```

### Comparing `netbox-tunnels2-0.2.1/setup.py` & `netbox-tunnels2-0.2.2/setup.py`

 * *Files identical despite different names*

