# Comparing `tmp/raster2dggs-0.1.1.tar.gz` & `tmp/raster2dggs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster2dggs-0.1.1.tar", max compression
+gzip compressed data, was "raster2dggs-0.1.2.tar", max compression
```

## Comparing `raster2dggs-0.1.1.tar` & `raster2dggs-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8160 2023-03-23 07:35:54.755193 raster2dggs-0.1.1/README.md
--rw-r--r--   0        0        0     1091 2023-03-23 07:35:54.770193 raster2dggs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 20:09:40.034837 raster2dggs-0.1.1/raster2dggs/__init__.py
--rw-r--r--   0        0        0      520 2023-03-15 20:09:40.034837 raster2dggs-0.1.1/raster2dggs/cli.py
--rw-r--r--   0        0        0    14499 2023-03-23 07:35:54.771193 raster2dggs-0.1.1/raster2dggs/h3.py
--rw-r--r--   0        0        0     9579 1970-01-01 00:00:00.000000 raster2dggs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     8160 2023-04-21 02:14:48.691969 raster2dggs-0.1.2/README.md
+-rw-r--r--   0        0        0     1091 2023-04-21 02:14:35.259789 raster2dggs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 20:09:40.034837 raster2dggs-0.1.2/raster2dggs/__init__.py
+-rw-r--r--   0        0        0      520 2023-03-15 20:09:40.034837 raster2dggs-0.1.2/raster2dggs/cli.py
+-rw-r--r--   0        0        0    14503 2023-04-21 02:05:36.690560 raster2dggs-0.1.2/raster2dggs/h3.py
+-rw-r--r--   0        0        0     9579 1970-01-01 00:00:00.000000 raster2dggs-0.1.2/PKG-INFO
```

### Comparing `raster2dggs-0.1.1/README.md` & `raster2dggs-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,17 @@
 ## Citation
 
 ```bibtex
 @software{raster2dggs,
   title={{raster2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/raster2dggs},
-  version={0.1.1},
+  version={0.1.2},
   date={2023-02-09}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). raster2dggs (0.1.1) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
+> Ardo, J., & Law, R. (2023). raster2dggs (0.1.2) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/raster2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `raster2dggs-0.1.1/pyproject.toml` & `raster2dggs-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raster2dggs"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/raster2dggs"
 keywords = ["dggs", "raster", "h3", "cli"]
```

### Comparing `raster2dggs-0.1.1/raster2dggs/cli.py` & `raster2dggs-0.1.2/raster2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `raster2dggs-0.1.1/raster2dggs/h3.py` & `raster2dggs-0.1.2/raster2dggs/h3.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     pandas .groupby function. This step is to ensure there are no duplicate h3 values, which will happen when indexing a
     high resolution raster at a coarser h3 resolution.
     """
     if decimals > 0:
         return df.groupby(f"h3_{resolution:02}").agg(aggfunc).round(decimals)
     else:
         return (
-            df.groupby(f"h3_{resolution:02}").agg(aggfunc).round(decimals).astype(int)
+            df.groupby(f"h3_{resolution:02}").agg(aggfunc).round(decimals).astype('Int64')
         )
 
 
 def _address_boundary_issues(
     pq_input: tempfile.TemporaryDirectory, output: Path, resolution: int, **kwargs
 ) -> Path:
     """
```

### Comparing `raster2dggs-0.1.1/PKG-INFO` & `raster2dggs-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster2dggs
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/manaakiwhenua/raster2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,raster,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -179,18 +179,18 @@
 ## Citation
 
 ```bibtex
 @software{raster2dggs,
   title={{raster2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/raster2dggs},
-  version={0.1.1},
+  version={0.1.2},
   date={2023-02-09}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). raster2dggs (0.1.1) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
+> Ardo, J., & Law, R. (2023). raster2dggs (0.1.2) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/raster2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

