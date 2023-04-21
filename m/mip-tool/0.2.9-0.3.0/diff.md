# Comparing `tmp/mip_tool-0.2.9-py3-none-any.whl.zip` & `tmp/mip_tool-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10551 bytes, number of entries: 10
+Zip file size: 10552 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      225 b- defN 80-Jan-01 00:00 mip_tool/__init__.py
 -rw-r--r--  2.0 unx     3050 b- defN 80-Jan-01 00:00 mip_tool/func/__init__.py
--rw-r--r--  2.0 unx     4852 b- defN 80-Jan-01 00:00 mip_tool/util.py
+-rw-r--r--  2.0 unx     4859 b- defN 80-Jan-01 00:00 mip_tool/util.py
 -rw-r--r--  2.0 unx     2237 b- defN 80-Jan-01 00:00 mip_tool/view/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 mip_tool/view/__main__.py
--rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 mip_tool-0.2.9.dist-info/LICENSE
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mip_tool-0.2.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 mip_tool-0.2.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     2638 b- defN 80-Jan-01 00:00 mip_tool-0.2.9.dist-info/METADATA
-?rw-r--r--  2.0 unx      788 b- defN 16-Jan-01 00:00 mip_tool-0.2.9.dist-info/RECORD
-10 files, 24709 bytes uncompressed, 9213 bytes compressed:  62.7%
+-rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 mip_tool-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mip_tool-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 mip_tool-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     2635 b- defN 80-Jan-01 00:00 mip_tool-0.3.0.dist-info/METADATA
+?rw-r--r--  2.0 unx      788 b- defN 16-Jan-01 00:00 mip_tool-0.3.0.dist-info/RECORD
+10 files, 24713 bytes uncompressed, 9214 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: mip_tool/view/__init__.py
 Comment: 
 
 Filename: mip_tool/view/__main__.py
 Comment: 
 
-Filename: mip_tool-0.2.9.dist-info/LICENSE
+Filename: mip_tool-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: mip_tool-0.2.9.dist-info/WHEEL
+Filename: mip_tool-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: mip_tool-0.2.9.dist-info/entry_points.txt
+Filename: mip_tool-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mip_tool-0.2.9.dist-info/METADATA
+Filename: mip_tool-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: mip_tool-0.2.9.dist-info/RECORD
+Filename: mip_tool-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mip_tool/util.py

```diff
@@ -28,15 +28,15 @@
     """
     return all(starmap(operator.ge, pairwise(it)))
 
 
 def add_line(m: Model, p1: Point, p2: Point, x: Var, y: Var, under: bool) -> None:
     """Add constraint which pass through p1 and p2.
 
-    :param m: Mpdel
+    :param m: Model
     :param p1: Point 1
     :param p2: Point 2
     :param x: Var x
     :param y: Var y
     :param under: 'y <= ...' if True, defaults to True
     """
     if dx := p2[0] - p1[0]:
@@ -44,15 +44,15 @@
         cx = p1[1] - p2[1]
         m += LinExpr([x, y], [cx, dx], const, "><"[int(under)])
 
 
 def add_lines_conv(m: Model, curve: np.ndarray, x: Var, y: Var, upward: bool = False):
     """Add convex piecewise linear constraint
 
-    :param m: Mpdel
+    :param m: Model
     :param curve: Point ndarray
     :param x: Var x
     :param y: Var y
     :param upward: Convex upward if True, defaults to False
     """
     tilt = np.divide(*np.diff(curve, axis=0).T[[1, 0]])
     if upward:
@@ -62,15 +62,15 @@
     for p1, p2 in pairwise(curve):
         add_line(m, p1, p2, x, y, upward)
 
 
 def add_lines(m: Model, curve: np.ndarray, x: Var, y: Var):
     """Add non-convex piecewise linear constraint
 
-    :param m: Mpdel
+    :param m: Model
     :param curve: Point ndarray
     :param x: Var x
     :param y: Var y
     """
     n = curve.shape[0]
     w = m.add_var_tensor((n - 1,), "w")
     z = m.add_var_tensor((n - 2,), "z", var_type="B")
@@ -140,15 +140,15 @@
     for v, e in zip(m.vars, np.eye(n)):
         lb = v.lb if v.lb > -1e308 else -np.inf
         ub = v.ub if v.ub < 1e308 else np.inf
         if not np.isinf([lb, ub]).all():
             yield list(e) + [lb, ub]
 
 
-def scipy_milp(m: Model, options: dict[str, Any] = None):
+def scipy_milp(m: Model, options: dict[str, Any] | None = None):
     """Solve by scipy.milp from mip.Model
 
     :param m: mip.Model
     :param options: options of scipy.milp, defaults to None
     :return: result of scipy.milp
     """
     from scipy.optimize import Bounds, LinearConstraint, milp
```

## Comparing `mip_tool-0.2.9.dist-info/LICENSE` & `mip_tool-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mip_tool-0.2.9.dist-info/METADATA` & `mip_tool-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mip-tool
-Version: 0.2.9
+Version: 0.3.0
 Summary: `mip-tool` is a package for Python-MIP.
 Home-page: https://github.com/SaitoTsutomu/mip-tool
 License: Apache-2.0
 Author: Saito Tsutomu
 Author-email: tsutomu7@hotmail.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Dist: mip (>=1.15,<2.0) ; python_version < "3.12"
-Requires-Dist: pandas (>=1.5,<2.0)
+Requires-Dist: pandas (>=1.5.3)
 Description-Content-Type: text/markdown
 
 # MIP-Tool
 
 MIP-Tool is a package for [Python-MIP](https://www.python-mip.com/).
 
 ## Installation
```

## Comparing `mip_tool-0.2.9.dist-info/RECORD` & `mip_tool-0.3.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 mip_tool/__init__.py,sha256=JBb14vsGl2rdhho0Qik2HZ_YeF-W9sRNqB7_h5W1WmE,225
 mip_tool/func/__init__.py,sha256=J6qHhJQ8YUb39YONlD9v_2lTYK8XOXSaaKmvYdOo9vs,3050
-mip_tool/util.py,sha256=RjqXlQvvNQKClOxhEnD0zLaP6NY2HqN9aDQBfJ1ko_Q,4852
+mip_tool/util.py,sha256=7cxolSiVz_r4rgyehBP9ShvbVyjwJwK8fB_JJ-tQhEI,4859
 mip_tool/view/__init__.py,sha256=TZ3MvnKq5Yt7uoe6JdkzqZuR7FRGSJftBL1HlbOkTq0,2237
 mip_tool/view/__main__.py,sha256=ubt6XyZvcHwdjCQ90B_U4MeP-3YJduz5GWUC9yOgkrg,27
-mip_tool-0.2.9.dist-info/LICENSE,sha256=P4wG11QaWXFTeHpKANPvc83droyjtsKJwzCAbzqFscA,10757
-mip_tool-0.2.9.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-mip_tool-0.2.9.dist-info/entry_points.txt,sha256=ov9UgbspHFzARW3m5ho2Y9M04iSmPAoTWT5WiTjNyQo,47
-mip_tool-0.2.9.dist-info/METADATA,sha256=6l0cDhe04pwhrStuy5a96XNZCvzYJrp3HZnFqRWwmt4,2638
-mip_tool-0.2.9.dist-info/RECORD,,
+mip_tool-0.3.0.dist-info/LICENSE,sha256=P4wG11QaWXFTeHpKANPvc83droyjtsKJwzCAbzqFscA,10757
+mip_tool-0.3.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+mip_tool-0.3.0.dist-info/entry_points.txt,sha256=ov9UgbspHFzARW3m5ho2Y9M04iSmPAoTWT5WiTjNyQo,47
+mip_tool-0.3.0.dist-info/METADATA,sha256=tTetgCaisLkcpfYtBkGxqbWaVSLezpUG4H1Wps92P5o,2635
+mip_tool-0.3.0.dist-info/RECORD,,
```

