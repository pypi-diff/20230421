# Comparing `tmp/caveclient-5.2.2.tar.gz` & `tmp/caveclient-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caveclient-5.2.2.tar", last modified: Fri Apr 21 14:32:47 2023, max compression
+gzip compressed data, was "caveclient-5.3.0.tar", last modified: Fri Apr 21 14:33:14 2023, max compression
```

## Comparing `caveclient-5.2.2.tar` & `caveclient-5.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:32:47.245154 caveclient-5.2.2/
--rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.2.2/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-21 14:32:47.244875 caveclient-5.2.2/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-03-24 04:01:05.000000 caveclient-5.2.2/README.rst
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:32:47.239417 caveclient-5.2.2/caveclient/
--rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-04-21 14:32:43.000000 caveclient-5.2.2/caveclient/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.2.2/caveclient/annotationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.2.2/caveclient/auth.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.2.2/caveclient/base.py
--rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-03-24 04:01:05.000000 caveclient-5.2.2/caveclient/chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-03-29 00:16:05.000000 caveclient-5.2.2/caveclient/datastack_lookup.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.2.2/caveclient/emannotationschemas.py
--rw-r--r--   0 forrestc   (503) staff       (20)    10436 2023-03-24 04:01:05.000000 caveclient-5.2.2/caveclient/endpoints.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-03-24 04:01:07.000000 caveclient-5.2.2/caveclient/format_utils.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-03-24 22:05:12.000000 caveclient-5.2.2/caveclient/frameworkclient.py
--rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.2.2/caveclient/infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.2.2/caveclient/jsonservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-03-24 04:01:07.000000 caveclient-5.2.2/caveclient/l2cache.py
--rw-r--r--   0 forrestc   (503) staff       (20)    77629 2023-04-21 14:32:40.000000 caveclient-5.2.2/caveclient/materializationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.2.2/caveclient/session_config.py
--rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.2.2/caveclient/timeit.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:32:47.241655 caveclient-5.2.2/caveclient/tools/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.2.2/caveclient/tools/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.2.2/caveclient/tools/caching.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.2.2/caveclient/tools/stage.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:32:47.240763 caveclient-5.2.2/caveclient.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-21 14:32:47.000000 caveclient-5.2.2/caveclient.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-04-21 14:32:47.000000 caveclient-5.2.2/caveclient.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-04-21 14:32:47.000000 caveclient-5.2.2/caveclient.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      115 2023-04-21 14:32:47.000000 caveclient-5.2.2/caveclient.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-04-21 14:32:47.000000 caveclient-5.2.2/caveclient.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      114 2022-12-21 20:12:16.000000 caveclient-5.2.2/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-04-21 14:32:47.245231 caveclient-5.2.2/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.2.2/setup.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:32:47.243224 caveclient-5.2.2/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.2.2/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-03-24 22:05:12.000000 caveclient-5.2.2/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.2.2/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.2.2/tests/test_chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.2.2/tests/test_infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.2.2/tests/test_materialization.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:33:14.838295 caveclient-5.3.0/
+-rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.3.0/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-21 14:33:14.837802 caveclient-5.3.0/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-03-24 04:01:05.000000 caveclient-5.3.0/README.rst
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:33:14.833866 caveclient-5.3.0/caveclient/
+-rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-04-21 14:33:11.000000 caveclient-5.3.0/caveclient/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.3.0/caveclient/annotationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.3.0/caveclient/auth.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.3.0/caveclient/base.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-03-24 04:01:05.000000 caveclient-5.3.0/caveclient/chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-03-29 00:16:05.000000 caveclient-5.3.0/caveclient/datastack_lookup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/emannotationschemas.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    10725 2023-04-21 14:33:06.000000 caveclient-5.3.0/caveclient/endpoints.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-03-24 04:01:07.000000 caveclient-5.3.0/caveclient/format_utils.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-03-24 22:05:12.000000 caveclient-5.3.0/caveclient/frameworkclient.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.3.0/caveclient/infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/jsonservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-03-24 04:01:07.000000 caveclient-5.3.0/caveclient/l2cache.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    85615 2023-04-21 14:33:06.000000 caveclient-5.3.0/caveclient/materializationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.3.0/caveclient/session_config.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/timeit.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:33:14.835595 caveclient-5.3.0/caveclient/tools/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/tools/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/tools/caching.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/tools/stage.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:33:14.834870 caveclient-5.3.0/caveclient.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-21 14:33:14.000000 caveclient-5.3.0/caveclient.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-04-21 14:33:14.000000 caveclient-5.3.0/caveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-04-21 14:33:14.000000 caveclient-5.3.0/caveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      115 2023-04-21 14:33:14.000000 caveclient-5.3.0/caveclient.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-04-21 14:33:14.000000 caveclient-5.3.0/caveclient.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      114 2022-12-21 20:12:16.000000 caveclient-5.3.0/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-04-21 14:33:14.838394 caveclient-5.3.0/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.3.0/setup.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:33:14.837473 caveclient-5.3.0/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.3.0/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-03-24 22:05:12.000000 caveclient-5.3.0/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.3.0/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.3.0/tests/test_chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.3.0/tests/test_infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.3.0/tests/test_materialization.py
```

### Comparing `caveclient-5.2.2/README.rst` & `caveclient-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/annotationengine.py` & `caveclient-5.3.0/caveclient/annotationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/auth.py` & `caveclient-5.3.0/caveclient/auth.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/base.py` & `caveclient-5.3.0/caveclient/base.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/chunkedgraph.py` & `caveclient-5.3.0/caveclient/chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/datastack_lookup.py` & `caveclient-5.3.0/caveclient/datastack_lookup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/emannotationschemas.py` & `caveclient-5.3.0/caveclient/emannotationschemas.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/endpoints.py` & `caveclient-5.3.0/caveclient/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,18 @@
     "ingest_annotation_table": mat_v2_api
     + "/materialize/run/ingest_annotations/datastack/{datastack_name}/{table_name}",
     "segmentation_metadata": mat_v3_api
     + "/datastack/{datastack_name}/table/{table_name}/segmentation_metadata",
     "live_live_query": mat_v3_api + "/datastack/{datastack_name}/query",
     "lookup_supervoxel_ids": mat_v2_api
     + "/materialize/run/lookup_svid/datastack/{datastack_name}/{table_name}",
+    "get_views": mat_v3_api + "/datastack/{datastack_name}/version/{version}/views",
+    "get_view_metadata": mat_v3_api + "/datastack/{datastack_name}/views/{view_name}/metadata",
+    "view_query": mat_v3_api
+    + "/datastack/{datastack_name}/version/{version}/views/{view_name}/query",
 }
 
 materialization_api_versions = {
     2: materialization_endpoints_v2,
     3: materialization_endpoints_v3,
 }
```

### Comparing `caveclient-5.2.2/caveclient/format_utils.py` & `caveclient-5.3.0/caveclient/format_utils.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/frameworkclient.py` & `caveclient-5.3.0/caveclient/frameworkclient.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/infoservice.py` & `caveclient-5.3.0/caveclient/infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/jsonservice.py` & `caveclient-5.3.0/caveclient/jsonservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/l2cache.py` & `caveclient-5.3.0/caveclient/l2cache.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/materializationengine.py` & `caveclient-5.3.0/caveclient/materializationengine.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,25 +461,30 @@
         filter_equal_dict,
         filter_spatial_dict,
         return_pyarrow,
         split_positions,
         offset,
         limit,
         desired_resolution,
+        use_view=False,
     ):
         endpoint_mapping = self.default_url_mapping
         endpoint_mapping["datastack_name"] = datastack_name
         endpoint_mapping["version"] = version
         data = {}
         query_args = {}
         query_args["return_pyarrow"] = return_pyarrow
         query_args["split_positions"] = split_positions
         if len(tables) == 1:
-            endpoint_mapping["table_name"] = tables[0]
-            url = self._endpoints["simple_query"].format_map(endpoint_mapping)
+            if use_view:
+                endpoint_mapping["view_name"] = tables[0]
+                url = self._endpoints["view_query"].format_map(endpoint_mapping)
+            else:
+                endpoint_mapping["table_name"] = tables[0]
+                url = self._endpoints["simple_query"].format_map(endpoint_mapping)
         else:
             data["tables"] = tables
             url = self._endpoints["join_query"].format_map(endpoint_mapping)
 
         if filter_in_dict is not None:
             data["filter_in_dict"] = filter_in_dict
         if filter_out_dict is not None:
@@ -1591,33 +1596,38 @@
 
         if remove_autapses:
             return df.query("pre_pt_root_id!=post_pt_root_id")
         else:
             return df
 
     def _assemble_attributes(
-        self, tables, suffixes=None, desired_resolution=None, **kwargs
+        self, tables, suffixes=None, desired_resolution=None, is_view=False, **kwargs
     ):
         if isinstance(tables, str):
             tables = [tables]
         if isinstance(desired_resolution, str):
             desired_resolution = np.array(
                 [float(r) for r in desired_resolution.split(", ")]
             )
         join_query = len(tables) > 1
 
         attrs = {
             "datastack_name": self.datastack_name,
         }
         if not join_query:
             attrs["join_query"] = False
-            try:
-                meta = self.get_table_metadata(tables[0], log_warning=False)
-            except:
-                meta = self.fc.annotation.get_table_metadata(tables[0])
+
+            if is_view:
+                meta = self.get_view_metadata(tables[0], log_warning=False)
+            else:
+                try:
+                    meta = self.get_table_metadata(tables[0], log_warning=False)
+                except:
+                    meta = self.fc.annotation.get_table_metadata(tables[0])
+
             for k, v in meta.items():
                 if re.match("^table", k):
                     attrs[k] = v
                 else:
                     attrs[f"table_{k}"] = v
             if desired_resolution is None:
                 attrs["dataframe_resolution"] = attrs["table_voxel_resolution"]
@@ -1842,13 +1852,180 @@
             except HTTPError as e:
                 raise Exception(
                     e.message
                     + " Metadata could not be loaded, try with metadata=False if not needed"
                 )
         return df
 
+    def get_views(self, version: int = None, datastack_name: str = None):
+        """get all available views for a version
+
+        Args:
+            version (int, optional): version to query.
+                                     Defaults to None. (will version set by client)
+            datastack_name (str, optional): datastack to query. Defaults to None.
+                                            (will use datastack set by client)
+
+        Returns:
+            list[str]: a list of views
+        """
+        if datastack_name is None:
+            datastack_name = self.datastack_name
+        if version is None:
+            version = self.version
+        endpoint_mapping = self.default_url_mapping
+        endpoint_mapping["datastack_name"] = datastack_name
+        endpoint_mapping["version"] = version 
+        url = self._endpoints["get_views"].format_map(endpoint_mapping)
+        response = self.session.get(url, verify=self.verify)
+        self.raise_for_status(response)
+        return response.json()
+
+    def get_view_metadata(self, view_name: str, log_warning: bool = True):
+        """get metadata for a view"""
+        endpoint_mapping = self.default_url_mapping
+        endpoint_mapping["view_name"] = view_name
+        url = self._endpoints["get_view_metadata"].format_map(endpoint_mapping)
+        response = self.session.get(url, verify=self.verify)
+        self.raise_for_status(response, log_warning=log_warning)
+        return response.json()
+
+    def query_view(
+        self,
+        view_name: str,
+        filter_in_dict=None,
+        filter_out_dict=None,
+        filter_equal_dict=None,
+        filter_spatial_dict=None,
+        select_columns=None,
+        offset: int = None,
+        limit: int = None,
+        datastack_name: str = None,
+        return_df: bool = True,
+        split_positions: bool = False,
+        materialization_version: int = None,
+        metadata: bool = True,
+        merge_reference: bool = True,
+        desired_resolution: Iterable = None,
+        get_counts: bool = False,
+    ):
+        """generic query on a view
+
+            Args:
+            table: 'str'
+
+            filter_in_dict (dict , optional):
+                keys are column names, values are allowed entries.
+                Defaults to None.
+            filter_out_dict (dict, optional):
+                keys are column names, values are not allowed entries.
+                Defaults to None.
+            filter_equal_dict (dict, optional):
+                inner layer: keys are column names, values are specified entry.
+                Defaults to None.
+            filter_spatial (dict, optional):
+                inner layer: keys are column names, values are bounding boxes
+                             as [[min_x, min_y,min_z],[max_x, max_y, max_z]]
+                             Expressed in units of the voxel_resolution of this dataset.
+            offset (int, optional): offset in query result
+            limit (int, optional): maximum results to return (server will set upper limit, see get_server_config)
+            select_columns (list of str, optional): columns to select. Defaults to None.
+            suffixes: (list[str], optional): suffixes to use on duplicate columns
+            offset (int, optional): result offset to use. Defaults to None.
+                will only return top K results.
+            datastack_name (str, optional): datastack to query.
+                If None defaults to one specified in client.
+            return_df (bool, optional): whether to return as a dataframe
+                default True, if False, data is returned as json (slower)
+            split_positions (bool, optional): whether to break position columns into x,y,z columns
+                default False, if False data is returned as one column with [x,y,z] array (slower)
+            materialization_version (int, optional): version to query.
+                If None defaults to one specified in client.
+            metadata: (bool, optional) : toggle to return metadata (default True)
+                If True (and return_df is also True), return table and query metadata in the df.attr dictionary.
+            merge_reference: (bool, optional) : toggle to automatically join reference table
+                If True, metadata will be queries and if its a reference table it will perform a join
+                on the reference table to return the rows of that
+            desired_resolution: (Iterable[float], Optional) : desired resolution you want all spatial points returned in
+                If None, defaults to one specified in client, if that is None then points are returned
+                as stored in the table and should be in the resolution specified in the table metadata
+        Returns:
+        pd.DataFrame: a pandas dataframe of results of query
+        """
+
+        if desired_resolution is None:
+            desired_resolution = self.desired_resolution
+        if materialization_version is None:
+            materialization_version = self.version
+        if datastack_name is None:
+            datastack_name = self.datastack_name
+
+        url, data, query_args, encoding = self._format_query_components(
+            datastack_name,
+            materialization_version,
+            [view_name],
+            select_columns,
+            None,
+            {view_name: filter_in_dict} if filter_in_dict is not None else None,
+            {view_name: filter_out_dict} if filter_out_dict is not None else None,
+            {view_name: filter_equal_dict} if filter_equal_dict is not None else None,
+            {view_name: filter_spatial_dict}
+            if filter_spatial_dict is not None
+            else None,
+            return_df,
+            True,
+            offset,
+            limit,
+            desired_resolution,
+            use_view=True,
+        )
+        if get_counts:
+            query_args["count"] = True
+        response = self.session.post(
+            url,
+            data=json.dumps(data, cls=BaseEncoder),
+            headers={"Content-Type": "application/json", "Accept-Encoding": encoding},
+            params=query_args,
+            stream=~return_df,
+        )
+        self.raise_for_status(response)
+        if return_df:
+            with warnings.catch_warnings():
+                warnings.simplefilter(action="ignore", category=FutureWarning)
+                warnings.simplefilter(action="ignore", category=DeprecationWarning)
+                df = pa.deserialize(response.content)
+                df = df.copy()
+
+            if metadata:
+                attrs = self._assemble_attributes(
+                    [view_name],
+                    filters={
+                        "inclusive": filter_in_dict,
+                        "exclusive": filter_out_dict,
+                        "equal": filter_equal_dict,
+                        "spatial": filter_spatial_dict,
+                    },
+                    select_columns=select_columns,
+                    offset=offset,
+                    limit=limit,
+                    live_query=False,
+                    timestamp=None,
+                    materialization_version=materialization_version,
+                    desired_resolution=response.headers.get(
+                        "dataframe_resolution", desired_resolution
+                    ),
+                    column_names=response.headers.get("column_names", None),
+                )
+                df.attrs.update(attrs)
+            if split_positions:
+                return df
+            else:
+                return concatenate_position_columns(df, inplace=True)
+        else:
+            return response.json()
+
 
 client_mapping = {
     2: MaterializatonClientV2,
     3: MaterializatonClientV3,
     "latest": MaterializatonClientV2,
 }
```

### Comparing `caveclient-5.2.2/caveclient/session_config.py` & `caveclient-5.3.0/caveclient/session_config.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/timeit.py` & `caveclient-5.3.0/caveclient/timeit.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/tools/caching.py` & `caveclient-5.3.0/caveclient/tools/caching.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient/tools/stage.py` & `caveclient-5.3.0/caveclient/tools/stage.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/caveclient.egg-info/SOURCES.txt` & `caveclient-5.3.0/caveclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/setup.py` & `caveclient-5.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/tests/conftest.py` & `caveclient-5.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/tests/test_annotation.py` & `caveclient-5.3.0/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/tests/test_chunkedgraph.py` & `caveclient-5.3.0/tests/test_chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/tests/test_infoservice.py` & `caveclient-5.3.0/tests/test_infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.2.2/tests/test_materialization.py` & `caveclient-5.3.0/tests/test_materialization.py`

 * *Files identical despite different names*

