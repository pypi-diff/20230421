# Comparing `tmp/spycio-0.2.4.tar.gz` & `tmp/spycio-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spycio-0.2.4.tar", max compression
+gzip compressed data, was "spycio-0.2.5.tar", max compression
```

## Comparing `spycio-0.2.4.tar` & `spycio-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-04-01 13:17:00.225289 spycio-0.2.4/LICENSE
--rw-r--r--   0        0        0     2824 2023-04-05 12:47:50.355077 spycio-0.2.4/README.md
--rw-r--r--   0        0        0     1376 2023-04-05 12:49:38.919501 spycio-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    14858 2023-04-01 13:17:00.225289 spycio-0.2.4/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb
--rw-r--r--   0        0        0      377 2023-04-02 20:20:51.957364 spycio-0.2.4/spycio/__init__.py
--rw-r--r--   0        0        0     4640 2023-04-05 11:40:15.343270 spycio-0.2.4/spycio/spycio.py
--rw-r--r--   0        0        0     3423 2023-04-05 01:00:51.299874 spycio-0.2.4/spycio/utils.py
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 spycio-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-01 13:17:00.225289 spycio-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2824 2023-04-05 12:47:50.355077 spycio-0.2.5/README.md
+-rw-r--r--   0        0        0     1376 2023-04-20 22:34:53.045430 spycio-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    14858 2023-04-01 13:17:00.225289 spycio-0.2.5/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb
+-rw-r--r--   0        0        0      377 2023-04-02 20:20:51.957364 spycio-0.2.5/spycio/__init__.py
+-rw-r--r--   0        0        0     7374 2023-04-20 22:16:11.949060 spycio-0.2.5/spycio/spycio.py
+-rw-r--r--   0        0        0     4368 2023-04-20 18:11:53.559951 spycio-0.2.5/spycio/utils.py
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 spycio-0.2.5/PKG-INFO
```

### Comparing `spycio-0.2.4/LICENSE` & `spycio-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spycio-0.2.4/README.md` & `spycio-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `spycio-0.2.4/pyproject.toml` & `spycio-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spycio"
-version = "0.2.4"
+version = "0.2.5"
 description = "Distances in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "spycio"}]
 homepage = "https://pypi.org/project/spycio/"
 repository = "https://github.com/trouchet/spycio"
```

### Comparing `spycio-0.2.4/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb` & `spycio-0.2.5/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `spycio-0.2.4/spycio/utils.py` & `spycio-0.2.5/spycio/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,33 +58,66 @@
   @param {Number} lng_degree
   @return {Number}
 '''
 def geoToSpher(lat_degree, lng_degree):
   return [pi/2 + degreeToRadian(lat_degree), pi + degreeToRadian(lng_degree)]
 
 '''
+  @abstract convert spherical coordinates into 
+  geographical coordinates a.k.a. latitude and longitude in degrees
+ 
+  @param {Number} lat_degree
+  @param {Number} lng_degree
+  @return {Number}
+'''
+def spherToGeo(coordinates):
+  return radianToDegree(coordinates[0]-pi/2), radianToDegree(coordinates[1]-pi)
+
+
+'''
+  @abstract an geographical coordinate of dimension n has:
+   1. Dimension equal 2;
+   2. Entries from index:
+     a. first entry  (latitude)  : between [-pi/2, pi/2];
+     b. second entry (longitude) : between [  -pi, pi];
+ 
+  @param {Array} u
+  @return {Boolean}
+'''
+def isGeographical(u):
+  hasLength2=lambda x: len(x)==2
+  isBetweenmmPI2andpPI2=lambda vec: vec[0] >= -90 and vec[0] <= 90
+  isBetweenmPIandpPI=lambda vec: vec[1] >= -180 and vec[1] <= 180
+  
+  print(hasLength2(u))
+  print(isBetweenmmPI2andpPI2(u))
+  print(isBetweenmPIandpPI(u))
+
+  return hasLength2(u) and isBetweenmmPI2andpPI2(u) and isBetweenmPIandpPI(u)
+
+'''
   @abstract an spherical coordinate of dimension n has:
    1. Dimension greater than 2;
    2. Entries from index:
      a. 0 to indexn-2 : between [-pi, pi];
      b. indexn-1      : between [0, 2 pi];
  
   @param {Array} u
   @return {Boolean}
 '''
 def isSpherical(u):
   u_length=len(u)
 
-  isBetweenmPIandpPI=lambda result, elem: result and elem >= 0 and elem <= pi
+  isBetween0andpPI=lambda result, elem: result and elem >= 0 and elem <= pi
   isBetween0and2PI=lambda result, elem: result and elem >= 0 and elem <= 2 * pi
   
-  areBetweenmPIandpPI=lambda vec: reduce(isBetweenmPIandpPI, vec, True)
+  areBetweenmPIandpPI=lambda vec: reduce(isBetween0andpPI, vec, True)
   areBetween0and2PI=lambda vec: reduce(isBetween0and2PI, vec, True)
 
-  return len(u) >= 2 and \
+  return u_length >= 2 and \
     areBetweenmPIandpPI(u[0:u_length - 1]) and\
     areBetween0and2PI(u[u_length - 1:u_length])
 
 '''
   @abstract converts map of spherical to cartesian coordinates
   The 3D representation order corresponds to (z, x, y)
```

### Comparing `spycio-0.2.4/PKG-INFO` & `spycio-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spycio
-Version: 0.2.4
+Version: 0.2.5
 Summary: Distances in python
 Home-page: https://pypi.org/project/spycio/
 License: MIT
 Keywords: distance
 Author: Bruno Peixoto
 Author-email: brunolnetto@gmail.com
 Requires-Python: >=3.8.1,<4.0
```

