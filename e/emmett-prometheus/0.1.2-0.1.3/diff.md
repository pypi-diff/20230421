# Comparing `tmp/emmett_prometheus-0.1.2.tar.gz` & `tmp/emmett_prometheus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett_prometheus-0.1.2.tar", max compression
+gzip compressed data, was "emmett_prometheus-0.1.3.tar", max compression
```

## Comparing `emmett_prometheus-0.1.2.tar` & `emmett_prometheus-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1486 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/LICENSE
--rw-r--r--   0        0        0     1831 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/README.md
--rw-r--r--   0        0        0       28 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/emmett_prometheus/__init__.py
--rw-r--r--   0        0        0       22 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/emmett_prometheus/__version__.py
--rw-r--r--   0        0        0     6067 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/emmett_prometheus/ext.py
--rw-r--r--   0        0        0     1369 2023-04-19 14:17:06.389055 emmett_prometheus-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 emmett_prometheus-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1831 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/README.md
+-rw-r--r--   0        0        0       28 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/emmett_prometheus/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/emmett_prometheus/__version__.py
+-rw-r--r--   0        0        0     6380 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/emmett_prometheus/ext.py
+-rw-r--r--   0        0        0     1369 2023-04-21 08:16:18.158111 emmett_prometheus-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 emmett_prometheus-0.1.3/PKG-INFO
```

### Comparing `emmett_prometheus-0.1.2/LICENSE` & `emmett_prometheus-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett_prometheus-0.1.2/README.md` & `emmett_prometheus-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `emmett_prometheus-0.1.2/emmett_prometheus/ext.py` & `emmett_prometheus-0.1.3/emmett_prometheus/ext.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,23 +81,30 @@
                 output='bytes'
             )(self._metrics_route)
 
     @listen_signal(Signals.before_route)
     def _inject_pipes(self, route, f):
         if not self.config.auto_load:
             return
-        if route.name in self._excluded_routes:
-            return
         if f == self._metrics_route:
             return
+        if self._get_route_name(route, f) in self._excluded_routes:
+            return
         if self.config.enable_http_metrics and isinstance(route, HTTPRoutingRule):
             route.pipeline.insert(0, self._pipe_http)
         if self.config.enable_ws_metrics and isinstance(route, WebsocketRoutingRule):
             route.pipeline.insert(0, self._pipe_ws)
 
+    @staticmethod
+    def _get_route_name(route, f):
+        rv = route.name or route.build_name(f)
+        if rv.endswith("."):
+            rv = rv + f.__name__
+        return rv
+
     async def _metrics_route(self):
         response.content_type = prometheus_client.exposition.CONTENT_TYPE_LATEST
         return prometheus_client.exposition.generate_latest(prometheus_client.REGISTRY)
 
 
 class PrometheusHTTPPipe(Pipe):
     def __init__(self, ext: Prometheus):
@@ -117,26 +124,32 @@
     async def close_request(self):
         self._http_counter.labels(
             route=request.name,
             method=request.method,
             status=response.status
         ).inc()
         if (
-            request.method not in self.ext._httph_filter_methods and
-            response.status in self.ext._httph_only_status
+            self.ext._httph_filter_methods and
+            request.method in self.ext._httph_filter_methods
+        ):
+            return
+        if (
+            self.ext._httph_only_status and
+            request.method not in self.ext._httph_only_status
         ):
-            self._http_histogram.labels(
-                route=request.name,
-                method=request.method,
-                status=response.status
-            ).observe(
-                (
-                    time.perf_counter_ns() - request._prometheus_http_histogram_ts
-                ) / 1_000_000
-            )
+            return
+        self._http_histogram.labels(
+            route=request.name,
+            method=request.method,
+            status=response.status
+        ).observe(
+            (
+                time.perf_counter_ns() - request._prometheus_http_histogram_ts
+            ) / 1_000_000
+        )
 
 
 class PrometheusWSPipe(Pipe):
     def __init__(self, ext: Prometheus):
         self.ext = ext
 
     @property
```

### Comparing `emmett_prometheus-0.1.2/pyproject.toml` & `emmett_prometheus-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett-prometheus"
-version = "0.1.2"
+version = "0.1.3"
 description = "Prometheus extension for Emmett framework"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/prometheus"
 repository = "https://github.com/emmett-framework/prometheus"
```

### Comparing `emmett_prometheus-0.1.2/PKG-INFO` & `emmett_prometheus-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett-prometheus
-Version: 0.1.2
+Version: 0.1.3
 Summary: Prometheus extension for Emmett framework
 Home-page: https://github.com/emmett-framework/prometheus
 License: BSD-3-Clause
 Keywords: prometheus,monitoring,emmett
 Author: Giovanni Barillari
 Author-email: g@baro.dev
 Requires-Python: >=3.8,<4.0
```

