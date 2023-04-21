# Comparing `tmp/odeanimate-0.0.8.tar.gz` & `tmp/odeanimate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odeanimate-0.0.8.tar", last modified: Thu Apr 20 15:40:10 2023, max compression
+gzip compressed data, was "odeanimate-0.0.9.tar", last modified: Thu Apr 20 17:35:36 2023, max compression
```

## Comparing `odeanimate-0.0.8.tar` & `odeanimate-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 15:40:10.163226 odeanimate-0.0.8/
--rw-r--r--   0 miguel.salgado   (501) staff       (20)    18092 2022-10-25 16:21:52.000000 odeanimate-0.0.8/LICENSE.txt
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     2714 2023-04-20 15:40:10.163066 odeanimate-0.0.8/PKG-INFO
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     1911 2023-04-03 04:36:58.000000 odeanimate-0.0.8/README.md
-drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 15:40:10.161141 odeanimate-0.0.8/odeanimate/
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      495 2023-04-20 15:39:41.000000 odeanimate-0.0.8/odeanimate/__init__.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)    12849 2023-04-20 15:39:20.000000 odeanimate-0.0.8/odeanimate/array.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     1846 2023-04-20 15:38:12.000000 odeanimate-0.0.8/odeanimate/codomain.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      241 2022-10-25 16:21:52.000000 odeanimate-0.0.8/odeanimate/constants.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)    11541 2023-04-04 04:17:56.000000 odeanimate-0.0.8/odeanimate/curve.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     9028 2022-10-25 16:21:52.000000 odeanimate-0.0.8/odeanimate/domains.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     2308 2023-03-31 05:23:44.000000 odeanimate-0.0.8/odeanimate/fields.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      233 2022-10-25 16:21:52.000000 odeanimate-0.0.8/odeanimate/jupyter.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     7255 2023-04-03 05:27:47.000000 odeanimate-0.0.8/odeanimate/matrix.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     4407 2022-10-25 16:21:52.000000 odeanimate-0.0.8/odeanimate/meta.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     3807 2023-03-14 04:53:39.000000 odeanimate-0.0.8/odeanimate/utils.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)    22340 2023-04-20 14:21:44.000000 odeanimate-0.0.8/odeanimate/vector.py
-drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 15:40:10.161988 odeanimate-0.0.8/odeanimate.egg-info/
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     2714 2023-04-20 15:40:10.000000 odeanimate-0.0.8/odeanimate.egg-info/PKG-INFO
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      586 2023-04-20 15:40:10.000000 odeanimate-0.0.8/odeanimate.egg-info/SOURCES.txt
--rw-r--r--   0 miguel.salgado   (501) staff       (20)        1 2023-04-20 15:40:10.000000 odeanimate-0.0.8/odeanimate.egg-info/dependency_links.txt
--rw-r--r--   0 miguel.salgado   (501) staff       (20)       11 2023-04-20 15:40:10.000000 odeanimate-0.0.8/odeanimate.egg-info/requires.txt
--rw-r--r--   0 miguel.salgado   (501) staff       (20)       11 2023-04-20 15:40:10.000000 odeanimate-0.0.8/odeanimate.egg-info/top_level.txt
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     1347 2023-04-20 14:18:41.000000 odeanimate-0.0.8/pyproject.toml
--rw-r--r--   0 miguel.salgado   (501) staff       (20)       38 2023-04-20 15:40:10.163278 odeanimate-0.0.8/setup.cfg
-drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 15:40:10.162838 odeanimate-0.0.8/tests/
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      571 2022-10-25 16:21:52.000000 odeanimate-0.0.8/tests/test_curves.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     1146 2023-04-20 15:31:20.000000 odeanimate-0.0.8/tests/test_trayectory.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     4236 2023-04-03 02:40:41.000000 odeanimate-0.0.8/tests/test_vector.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)      132 2023-03-31 05:23:44.000000 odeanimate-0.0.8/tests/test_vector_2d.py
--rw-r--r--   0 miguel.salgado   (501) staff       (20)     1533 2022-10-25 16:21:52.000000 odeanimate-0.0.8/tests/test_vector_from_methods.py
+drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 17:35:36.417240 odeanimate-0.0.9/
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)    18092 2022-10-25 16:21:52.000000 odeanimate-0.0.9/LICENSE.txt
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     2618 2023-04-20 17:35:36.417002 odeanimate-0.0.9/PKG-INFO
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     1815 2023-04-20 17:29:49.000000 odeanimate-0.0.9/README.md
+drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 17:35:36.414189 odeanimate-0.0.9/odeanimate/
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      495 2023-04-20 17:29:49.000000 odeanimate-0.0.9/odeanimate/__init__.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)    12849 2023-04-20 17:29:49.000000 odeanimate-0.0.9/odeanimate/array.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     1846 2023-04-20 17:29:49.000000 odeanimate-0.0.9/odeanimate/codomain.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      241 2022-10-25 16:21:52.000000 odeanimate-0.0.9/odeanimate/constants.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)    11541 2023-04-20 17:29:49.000000 odeanimate-0.0.9/odeanimate/curve.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     9028 2022-10-25 16:21:52.000000 odeanimate-0.0.9/odeanimate/domains.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     2308 2023-04-20 17:29:49.000000 odeanimate-0.0.9/odeanimate/fields.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      233 2022-10-25 16:21:52.000000 odeanimate-0.0.9/odeanimate/jupyter.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     7255 2023-04-20 17:29:49.000000 odeanimate-0.0.9/odeanimate/matrix.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     4515 2023-04-20 17:29:49.000000 odeanimate-0.0.9/odeanimate/meta.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     3851 2023-04-20 17:29:49.000000 odeanimate-0.0.9/odeanimate/utils.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)    22340 2023-04-20 17:29:49.000000 odeanimate-0.0.9/odeanimate/vector.py
+drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 17:35:36.415672 odeanimate-0.0.9/odeanimate.egg-info/
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     2618 2023-04-20 17:35:36.000000 odeanimate-0.0.9/odeanimate.egg-info/PKG-INFO
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      586 2023-04-20 17:35:36.000000 odeanimate-0.0.9/odeanimate.egg-info/SOURCES.txt
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)        1 2023-04-20 17:35:36.000000 odeanimate-0.0.9/odeanimate.egg-info/dependency_links.txt
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)       11 2023-04-20 17:35:36.000000 odeanimate-0.0.9/odeanimate.egg-info/requires.txt
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)       11 2023-04-20 17:35:36.000000 odeanimate-0.0.9/odeanimate.egg-info/top_level.txt
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     1347 2023-04-20 17:29:49.000000 odeanimate-0.0.9/pyproject.toml
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)       38 2023-04-20 17:35:36.417353 odeanimate-0.0.9/setup.cfg
+drwxr-xr-x   0 miguel.salgado   (501) staff       (20)        0 2023-04-20 17:35:36.416752 odeanimate-0.0.9/tests/
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      571 2022-10-25 16:21:52.000000 odeanimate-0.0.9/tests/test_curves.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     1146 2023-04-20 17:29:49.000000 odeanimate-0.0.9/tests/test_trayectory.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     4236 2023-04-20 17:29:49.000000 odeanimate-0.0.9/tests/test_vector.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)      132 2023-04-20 17:29:49.000000 odeanimate-0.0.9/tests/test_vector_2d.py
+-rw-r--r--   0 miguel.salgado   (501) staff       (20)     1533 2022-10-25 16:21:52.000000 odeanimate-0.0.9/tests/test_vector_from_methods.py
```

### Comparing `odeanimate-0.0.8/LICENSE.txt` & `odeanimate-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/PKG-INFO` & `odeanimate-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odeanimate
-Version: 0.0.8
+Version: 0.0.9
 Summary: A module for useful quick mathematical calculation, plotting and animation.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://odeanimate.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/odeanimate
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
@@ -26,15 +26,14 @@
 > The rational for this is, _trying to use pure-python_ to do numerical analysis.
 
 Most techniques here are going to be without the use of any external modules.
 
 The only external modules that are used _directly_ by this project are:
 
  - `matplotlib`, which is used to configure the _figures_ for plotting.
- - `ffmpeg-python`, which is used to _gather_ several _figures_ and turn them in to animations.
 
 
 ## Features
 
 > Most of this features are _W.I.P._ (work in progress)
 
  - [x] Vector objects with _basic_ operations.
```

### Comparing `odeanimate-0.0.8/README.md` & `odeanimate-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 > The rational for this is, _trying to use pure-python_ to do numerical analysis.
 
 Most techniques here are going to be without the use of any external modules.
 
 The only external modules that are used _directly_ by this project are:
 
  - `matplotlib`, which is used to configure the _figures_ for plotting.
- - `ffmpeg-python`, which is used to _gather_ several _figures_ and turn them in to animations.
 
 
 ## Features
 
 > Most of this features are _W.I.P._ (work in progress)
 
  - [x] Vector objects with _basic_ operations.
```

### Comparing `odeanimate-0.0.8/odeanimate/array.py` & `odeanimate-0.0.9/odeanimate/array.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/odeanimate/codomain.py` & `odeanimate-0.0.9/odeanimate/codomain.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/odeanimate/curve.py` & `odeanimate-0.0.9/odeanimate/curve.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/odeanimate/domains.py` & `odeanimate-0.0.9/odeanimate/domains.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/odeanimate/fields.py` & `odeanimate-0.0.9/odeanimate/fields.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/odeanimate/matrix.py` & `odeanimate-0.0.9/odeanimate/matrix.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/odeanimate/meta.py` & `odeanimate-0.0.9/odeanimate/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 
 class MathematicalFunction:
     domain = None
     codomain = None
     _keys = None
 
-    def __init__(self, function=None, domain=None, codomain=None, keys=None, **kwargs):
+    def __init__(
+        self, function=None, domain=None, codomain=None, keys=None, **kwargs
+    ):
         if domain is not None:
             self.domain = domain
         elif self.domain is None:
             raise Exception("No domain configured")
 
         if codomain is not None:
             self.codomain = codomain
@@ -49,17 +51,23 @@
                 _returnable = self._function(nargs, **kwargs)
             if _returnable is None:
                 raise Exception("Error evaluating function")
             return self.codomain.from_compatible(_returnable)
 
     def __add__(self, other):
         _new_func, cls = None, None
-        if isinstance(other, MathematicalFunction) and self.domain != other.domain:
+        if (
+            isinstance(other, MathematicalFunction)
+            and self.domain != other.domain
+        ):
             raise Exception("Incompatible domains")
-        if isinstance(other, self.__class__) and self.codomain == other.codomain:
+        if (
+            isinstance(other, self.__class__)
+            and self.codomain == other.codomain
+        ):
 
             def _new_func(*args, **kwargs):
                 return self(*args, **kwargs) + other(*args, **kwargs)
 
             cls = self.__class__
 
         elif self.codomain.is_compatible(other):
@@ -102,15 +110,17 @@
         Scalar x Vector = Vector
         Vector x Scalar = Vector
         """
         _new_func, cls = None, None
         if self.domain != other.domain:
             raise Exception("Incompatible domains")
 
-        if self.codomain.is_compatible(other) or RealNumber.is_compatible(other):
+        if self.codomain.is_compatible(other) or RealNumber.is_compatible(
+            other
+        ):
 
             def _new_func(*args, **kwargs):
                 return self(*args, **kwargs) * other
 
             cls = self.__class__
 
         if (
```

### Comparing `odeanimate-0.0.8/odeanimate/utils.py` & `odeanimate-0.0.9/odeanimate/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,16 +130,20 @@
     def __call__(self, t):
         if t in self.values.keys():
             return self.values[t]
         m, M = self.limits
         if t > M or t < m:
             raise Exception("Out of bound")
 
-        lower = min(filter(lambda k: k < self.values.keys()), key=lambda k: abs(t - k))
-        upper = min(filter(lambda k: k > self.values.keys()), key=lambda k: abs(t - k))
+        lower = min(
+            filter(lambda k: k < self.values.keys()), key=lambda k: abs(t - k)
+        )
+        upper = min(
+            filter(lambda k: k > self.values.keys()), key=lambda k: abs(t - k)
+        )
         return t * (self.values[upper] - self.values[lower]) / (upper - lower)
 
     @property
     def limits(self):
         return (
             min(self.values.keys()),
             max(self.values.keys()),
```

### Comparing `odeanimate-0.0.8/odeanimate/vector.py` & `odeanimate-0.0.9/odeanimate/vector.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/odeanimate.egg-info/PKG-INFO` & `odeanimate-0.0.9/odeanimate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odeanimate
-Version: 0.0.8
+Version: 0.0.9
 Summary: A module for useful quick mathematical calculation, plotting and animation.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://odeanimate.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/odeanimate
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
@@ -26,15 +26,14 @@
 > The rational for this is, _trying to use pure-python_ to do numerical analysis.
 
 Most techniques here are going to be without the use of any external modules.
 
 The only external modules that are used _directly_ by this project are:
 
  - `matplotlib`, which is used to configure the _figures_ for plotting.
- - `ffmpeg-python`, which is used to _gather_ several _figures_ and turn them in to animations.
 
 
 ## Features
 
 > Most of this features are _W.I.P._ (work in progress)
 
  - [x] Vector objects with _basic_ operations.
```

### Comparing `odeanimate-0.0.8/odeanimate.egg-info/SOURCES.txt` & `odeanimate-0.0.9/odeanimate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/pyproject.toml` & `odeanimate-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/tests/test_curves.py` & `odeanimate-0.0.9/tests/test_curves.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/tests/test_trayectory.py` & `odeanimate-0.0.9/tests/test_trayectory.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/tests/test_vector.py` & `odeanimate-0.0.9/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `odeanimate-0.0.8/tests/test_vector_from_methods.py` & `odeanimate-0.0.9/tests/test_vector_from_methods.py`

 * *Files identical despite different names*

