# Comparing `tmp/geostat-0.8.2.tar.gz` & `tmp/geostat-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/whdc/git/geostat/dist/.tmp-399ucofq/geostat-0.8.2.tar", last modified: Mon Apr 17 00:52:28 2023, max compression
+gzip compressed data, was "/home/whdc/git/geostat/dist/.tmp-q5pzns9y/geostat-0.8.3.tar", last modified: Fri Apr 21 18:09:19 2023, max compression
```

## Comparing `geostat-0.8.2.tar` & `geostat-0.8.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-17 00:52:28.076028 geostat-0.8.2/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2022-08-12 07:59:13.000000 geostat-0.8.2/LICENSE
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-17 00:52:28.076028 geostat-0.8.2/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2022-08-12 07:59:13.000000 geostat-0.8.2/README.md
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      679 2023-04-17 00:49:58.000000 geostat-0.8.2/pyproject.toml
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      926 2023-04-17 00:52:28.076028 geostat-0.8.2/setup.cfg
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-17 00:52:28.072028 geostat-0.8.2/src/
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-17 00:52:28.076028 geostat-0.8.2/src/geostat/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-04-17 00:49:50.000000 geostat-0.8.2/src/geostat/__init__.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    16688 2023-04-17 00:19:52.000000 geostat-0.8.2/src/geostat/kernel.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-03-05 02:04:42.000000 geostat-0.8.2/src/geostat/krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-10 22:02:47.000000 geostat-0.8.2/src/geostat/mean.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2022-08-16 21:11:34.000000 geostat-0.8.2/src/geostat/mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-03-05 02:04:42.000000 geostat-0.8.2/src/geostat/metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    22135 2023-04-10 22:15:32.000000 geostat-0.8.2/src/geostat/model.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3424 2023-04-10 21:29:01.000000 geostat-0.8.2/src/geostat/op.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3167 2023-04-12 00:49:25.000000 geostat-0.8.2/src/geostat/param.py
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-17 00:52:28.076028 geostat-0.8.2/src/geostat.egg-info/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-17 00:52:28.000000 geostat-0.8.2/src/geostat.egg-info/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      592 2023-04-17 00:52:28.000000 geostat-0.8.2/src/geostat.egg-info/SOURCES.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-04-17 00:52:28.000000 geostat-0.8.2/src/geostat.egg-info/dependency_links.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-04-17 00:52:28.000000 geostat-0.8.2/src/geostat.egg-info/requires.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-04-17 00:52:28.000000 geostat-0.8.2/src/geostat.egg-info/top_level.txt
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-17 00:52:28.076028 geostat-0.8.2/tests/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-10 21:29:01.000000 geostat-0.8.2/tests/test_antiderivative.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-10 22:36:21.000000 geostat-0.8.2/tests/test_delta.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-04-10 21:29:01.000000 geostat-0.8.2/tests/test_gp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2022-08-12 07:59:13.000000 geostat-0.8.2/tests/test_krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-10 22:36:43.000000 geostat-0.8.2/tests/test_mcmc.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2022-08-12 08:18:35.000000 geostat-0.8.2/tests/test_mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-10 21:50:09.000000 geostat-0.8.2/tests/test_metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-10 22:14:06.000000 geostat-0.8.2/tests/test_multigp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-10 21:52:59.000000 geostat-0.8.2/tests/test_trend.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-21 18:09:19.382182 geostat-0.8.3/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2022-08-12 07:59:13.000000 geostat-0.8.3/LICENSE
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-21 18:09:19.382182 geostat-0.8.3/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2022-08-12 07:59:13.000000 geostat-0.8.3/README.md
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      679 2023-04-21 15:52:57.000000 geostat-0.8.3/pyproject.toml
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      926 2023-04-21 18:09:19.382182 geostat-0.8.3/setup.cfg
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-21 18:09:19.378182 geostat-0.8.3/src/
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-21 18:09:19.382182 geostat-0.8.3/src/geostat/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-04-21 15:51:28.000000 geostat-0.8.3/src/geostat/__init__.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    18354 2023-04-21 15:51:20.000000 geostat-0.8.3/src/geostat/kernel.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-03-05 02:04:42.000000 geostat-0.8.3/src/geostat/krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-10 22:02:47.000000 geostat-0.8.3/src/geostat/mean.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2022-08-16 21:11:34.000000 geostat-0.8.3/src/geostat/mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-03-05 02:04:42.000000 geostat-0.8.3/src/geostat/metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    22135 2023-04-10 22:15:32.000000 geostat-0.8.3/src/geostat/model.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3424 2023-04-10 21:29:01.000000 geostat-0.8.3/src/geostat/op.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3167 2023-04-12 00:49:25.000000 geostat-0.8.3/src/geostat/param.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-21 18:09:19.382182 geostat-0.8.3/src/geostat.egg-info/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-21 18:09:19.000000 geostat-0.8.3/src/geostat.egg-info/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      592 2023-04-21 18:09:19.000000 geostat-0.8.3/src/geostat.egg-info/SOURCES.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-04-21 18:09:19.000000 geostat-0.8.3/src/geostat.egg-info/dependency_links.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-04-21 18:09:19.000000 geostat-0.8.3/src/geostat.egg-info/requires.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-04-21 18:09:19.000000 geostat-0.8.3/src/geostat.egg-info/top_level.txt
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-21 18:09:19.382182 geostat-0.8.3/tests/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-10 21:29:01.000000 geostat-0.8.3/tests/test_antiderivative.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-10 22:36:21.000000 geostat-0.8.3/tests/test_delta.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-04-10 21:29:01.000000 geostat-0.8.3/tests/test_gp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2022-08-12 07:59:13.000000 geostat-0.8.3/tests/test_krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-10 22:36:43.000000 geostat-0.8.3/tests/test_mcmc.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2022-08-12 08:18:35.000000 geostat-0.8.3/tests/test_mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-10 21:50:09.000000 geostat-0.8.3/tests/test_metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-10 22:14:06.000000 geostat-0.8.3/tests/test_multigp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-10 21:52:59.000000 geostat-0.8.3/tests/test_trend.py
```

### Comparing `geostat-0.8.2/LICENSE` & `geostat-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/PKG-INFO` & `geostat-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.8.2
+Version: 0.8.3
 Summary: Model spatial data with Gaussian processes
 Home-page: https://code.usgs.gov/mjstephens/geostat
 Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `geostat-0.8.2/README.md` & `geostat-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/pyproject.toml` & `geostat-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geostat"
-version = "0.8.2"
+version = "0.8.3"
 description = "Model spatial data with Gaussian processes"
 readme = "README.md"
 authors = [
   {name="Michael J. Stephens", email="mjstephens@usgs.gov"},
   {name="Will Chang", email="will@hypergradient.ai"}
 ]
 license = { file = "LICENSE" }
```

### Comparing `geostat-0.8.2/setup.cfg` & `geostat-0.8.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geostat
-version = 0.8.2
+version = 0.8.3
 author = Michael J. Stephens, Will Chang
 author_email = mjstephens@usgs.gov, will@hypergradient.ai
 description = Python package for performing kriging and Gaussian processes with geoscience-oriented utilities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://code.usgs.gov/mjstephens/geostat
 project_urls =
```

### Comparing `geostat-0.8.2/src/geostat/kernel.py` & `geostat-0.8.3/src/geostat/kernel.py`

 * *Files 5% similar despite different names*

```diff
@@ -206,14 +206,58 @@
 
         return rampstack(tf.sqrt(e['d2']), v['sill'], v['range'])
 
     def reg(self, p):
         v = get_parameter_values(self.fa, p)
         return v['range']
 
+@tf.custom_gradient
+def quadstack(x, sills, ranges):
+    """
+    `x` has arbitrary shape [...], but must be non-negative.
+    `sills` and `ranges` both have shape [K].
+    """
+    ex = ed(x)
+    ax = tf.maximum(0., 1. - tf.abs(ex) / ranges) # [..., 1]
+    y = sills * tf.square(ax) # [..., K]
+    def grad(upstream):
+        ex = ed(x)
+        ax = tf.maximum(0., 1. - tf.abs(ex) / ranges) # [..., 1]
+        y = sills * tf.square(ax) # [..., K]
+        sx = tf.sign(ex)
+        gx = sx * ax * (-2. * sills / ranges) 
+        K = tf.shape(sills)[0]
+        grad_x = upstream * tf.reduce_sum(gx, -1) # [...]
+        grad_sills = tf.einsum('ak,a->k', tf.reshape(y, [-1, K]), tf.reshape(upstream, [-1]))
+        grad_ranges = tf.einsum('ak,a->k', tf.reshape(-gx / ranges, [-1, K]), tf.reshape(upstream, [-1]))
+        return grad_x, grad_sills, grad_ranges
+    return tf.reduce_sum(y, -1), grad
+
+class QuadStack(Kernel):
+    def __init__(self, range='range', sill='sill', scale=None, metric=None):
+        fa = dict(sill=sill, range=range, scale=scale)
+        autoinputs = scale_to_metric(scale, metric)
+        super().__init__(fa, dict(d2=autoinputs))
+
+    def vars(self):
+        return ppp_list(self.fa['sill']) + ppp_list(self.fa['range'])
+
+    def call(self, p, e):
+        v = get_parameter_values(self.fa, p)
+        if isinstance(v['sill'], (tuple, list)):
+            v['sill'] = tf.stack(v['sill'])
+        if isinstance(v['range'], (tuple, list)):
+            v['range'] = tf.stack(v['range'])
+
+        return quadstack(tf.sqrt(e['d2']), v['sill'], v['range'])
+
+    def reg(self, p):
+        v = get_parameter_values(self.fa, p)
+        return v['range']
+
 class Wiener(Kernel):
     def __init__(self, axis, start):
 
         self.axis = axis
         self.start = start
 
         # Include the element of scale corresponding to the axis of
```

### Comparing `geostat-0.8.2/src/geostat/krige.py` & `geostat-0.8.3/src/geostat/krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/src/geostat/mean.py` & `geostat-0.8.3/src/geostat/mean.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/src/geostat/mesh.py` & `geostat-0.8.3/src/geostat/mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/src/geostat/metric.py` & `geostat-0.8.3/src/geostat/metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/src/geostat/model.py` & `geostat-0.8.3/src/geostat/model.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/src/geostat/op.py` & `geostat-0.8.3/src/geostat/op.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/src/geostat/param.py` & `geostat-0.8.3/src/geostat/param.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/src/geostat.egg-info/PKG-INFO` & `geostat-0.8.3/src/geostat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.8.2
+Version: 0.8.3
 Summary: Model spatial data with Gaussian processes
 Home-page: https://code.usgs.gov/mjstephens/geostat
 Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `geostat-0.8.2/src/geostat.egg-info/SOURCES.txt` & `geostat-0.8.3/src/geostat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/tests/test_antiderivative.py` & `geostat-0.8.3/tests/test_antiderivative.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/tests/test_delta.py` & `geostat-0.8.3/tests/test_delta.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/tests/test_gp.py` & `geostat-0.8.3/tests/test_gp.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/tests/test_krige.py` & `geostat-0.8.3/tests/test_krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/tests/test_mcmc.py` & `geostat-0.8.3/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/tests/test_mesh.py` & `geostat-0.8.3/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/tests/test_metric.py` & `geostat-0.8.3/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/tests/test_multigp.py` & `geostat-0.8.3/tests/test_multigp.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.2/tests/test_trend.py` & `geostat-0.8.3/tests/test_trend.py`

 * *Files identical despite different names*

