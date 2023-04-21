# Comparing `tmp/sketchlib-0.0.0.tar.gz` & `tmp/sketchlib-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sketchlib-0.0.0.tar", last modified: Fri Apr 21 04:45:07 2023, max compression
+gzip compressed data, was "sketchlib-0.0.1.tar", last modified: Fri Apr 21 05:25:16 2023, max compression
```

## Comparing `sketchlib-0.0.0.tar` & `sketchlib-0.0.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 04:45:07.417386 sketchlib-0.0.0/
--rw-rw-rw-   0        0        0     1107 2023-04-20 19:32:39.000000 sketchlib-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     2137 2023-04-21 04:45:07.414395 sketchlib-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-21 04:41:49.000000 sketchlib-0.0.0/README.md
--rw-rw-rw-   0        0        0     1307 2023-04-21 04:41:29.000000 sketchlib-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 04:45:07.417386 sketchlib-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 04:45:07.375653 sketchlib-0.0.0/sketchlib.egg-info/
--rw-rw-rw-   0        0        0     2137 2023-04-21 04:45:07.000000 sketchlib-0.0.0/sketchlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-04-21 04:45:07.000000 sketchlib-0.0.0/sketchlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 04:45:07.000000 sketchlib-0.0.0/sketchlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-21 04:45:07.000000 sketchlib-0.0.0/sketchlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-21 04:45:07.000000 sketchlib-0.0.0/sketchlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 04:45:07.401385 sketchlib-0.0.0/streamsketchlib/
--rw-rw-rw-   0        0        0        0 2023-03-27 18:18:54.000000 sketchlib-0.0.0/streamsketchlib/__init__.py
--rw-rw-rw-   0        0        0     1205 2023-04-18 22:00:01.000000 sketchlib-0.0.0/streamsketchlib/bloom_filter.py
--rw-rw-rw-   0        0        0     3581 2023-04-20 22:33:06.000000 sketchlib-0.0.0/streamsketchlib/cm_hh_cash_register.py
--rw-rw-rw-   0        0        0     2399 2023-04-14 18:07:20.000000 sketchlib-0.0.0/streamsketchlib/count_min.py
--rw-rw-rw-   0        0        0     2326 2023-03-27 17:31:29.000000 sketchlib-0.0.0/streamsketchlib/f0_bjkst.py
--rw-rw-rw-   0        0        0     3267 2023-04-13 23:38:23.000000 sketchlib-0.0.0/streamsketchlib/f0_estimate.py
--rw-rw-rw-   0        0        0     2104 2023-04-13 23:38:23.000000 sketchlib-0.0.0/streamsketchlib/f2_estimate.py
--rw-rw-rw-   0        0        0      744 2023-04-20 22:40:57.000000 sketchlib-0.0.0/streamsketchlib/heavy_hitters.py
--rw-rw-rw-   0        0        0     1935 2023-04-14 19:30:34.000000 sketchlib-0.0.0/streamsketchlib/heavy_hitters_cm.py
--rw-rw-rw-   0        0        0     3690 2023-03-27 17:31:29.000000 sketchlib-0.0.0/streamsketchlib/minhash.py
--rw-rw-rw-   0        0        0     4296 2023-03-27 17:31:29.000000 sketchlib-0.0.0/streamsketchlib/misra_gries.py
--rw-rw-rw-   0        0        0      788 2023-03-30 20:22:20.000000 sketchlib-0.0.0/streamsketchlib/rsv_sampling.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:45:07.413386 sketchlib-0.0.0/tests/
--rw-rw-rw-   0        0        0     3134 2023-04-20 21:27:51.000000 sketchlib-0.0.0/tests/test_bloom_filter.py
--rw-rw-rw-   0        0        0     2197 2023-04-11 22:11:29.000000 sketchlib-0.0.0/tests/test_count_min.py
--rw-rw-rw-   0        0        0     1479 2023-03-30 20:16:29.000000 sketchlib-0.0.0/tests/test_f0_estimate.py
--rw-rw-rw-   0        0        0     1043 2023-03-30 22:04:32.000000 sketchlib-0.0.0/tests/test_f2_estimate.py
--rw-rw-rw-   0        0        0     4197 2023-04-14 18:07:20.000000 sketchlib-0.0.0/tests/test_hh_count_min.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:25:16.753268 sketchlib-0.0.1/
+-rw-rw-rw-   0        0        0     1107 2023-04-20 19:32:39.000000 sketchlib-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2137 2023-04-21 05:25:16.752251 sketchlib-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-21 05:06:35.000000 sketchlib-0.0.1/README.md
+-rw-rw-rw-   0        0        0     1238 2023-04-21 05:24:00.000000 sketchlib-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 05:25:16.753268 sketchlib-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 05:25:16.701661 sketchlib-0.0.1/sketchlib.egg-info/
+-rw-rw-rw-   0        0        0     2137 2023-04-21 05:25:16.000000 sketchlib-0.0.1/sketchlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2023-04-21 05:25:16.000000 sketchlib-0.0.1/sketchlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 05:25:16.000000 sketchlib-0.0.1/sketchlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-21 05:25:16.000000 sketchlib-0.0.1/sketchlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-21 05:25:16.000000 sketchlib-0.0.1/sketchlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 05:25:16.734638 sketchlib-0.0.1/streamsketchlib/
+-rw-rw-rw-   0        0        0        0 2023-03-27 18:18:54.000000 sketchlib-0.0.1/streamsketchlib/__init__.py
+-rw-rw-rw-   0        0        0     1205 2023-04-18 22:00:01.000000 sketchlib-0.0.1/streamsketchlib/bloom_filter.py
+-rw-rw-rw-   0        0        0     3493 2023-04-21 05:04:12.000000 sketchlib-0.0.1/streamsketchlib/cm_hh_cash_register.py
+-rw-rw-rw-   0        0        0     2399 2023-04-14 18:07:20.000000 sketchlib-0.0.1/streamsketchlib/count_min.py
+-rw-rw-rw-   0        0        0     2326 2023-03-27 17:31:29.000000 sketchlib-0.0.1/streamsketchlib/f0_bjkst.py
+-rw-rw-rw-   0        0        0     3267 2023-04-13 23:38:23.000000 sketchlib-0.0.1/streamsketchlib/f0_estimate.py
+-rw-rw-rw-   0        0        0     2104 2023-04-13 23:38:23.000000 sketchlib-0.0.1/streamsketchlib/f2_estimate.py
+-rw-rw-rw-   0        0        0     1935 2023-04-14 19:30:34.000000 sketchlib-0.0.1/streamsketchlib/heavy_hitters_cm.py
+-rw-rw-rw-   0        0        0     3690 2023-03-27 17:31:29.000000 sketchlib-0.0.1/streamsketchlib/minhash.py
+-rw-rw-rw-   0        0        0     4296 2023-03-27 17:31:29.000000 sketchlib-0.0.1/streamsketchlib/misra_gries.py
+-rw-rw-rw-   0        0        0      788 2023-03-30 20:22:20.000000 sketchlib-0.0.1/streamsketchlib/rsv_sampling.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:25:16.750254 sketchlib-0.0.1/tests/
+-rw-rw-rw-   0        0        0     3134 2023-04-20 21:27:51.000000 sketchlib-0.0.1/tests/test_bloom_filter.py
+-rw-rw-rw-   0        0        0     2197 2023-04-11 22:11:29.000000 sketchlib-0.0.1/tests/test_count_min.py
+-rw-rw-rw-   0        0        0     1479 2023-03-30 20:16:29.000000 sketchlib-0.0.1/tests/test_f0_estimate.py
+-rw-rw-rw-   0        0        0     1043 2023-03-30 22:04:32.000000 sketchlib-0.0.1/tests/test_f2_estimate.py
+-rw-rw-rw-   0        0        0     4197 2023-04-14 18:07:20.000000 sketchlib-0.0.1/tests/test_hh_count_min.py
```

### Comparing `sketchlib-0.0.0/LICENSE` & `sketchlib-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/PKG-INFO` & `sketchlib-0.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchlib
-Version: 0.0.0
+Version: 0.0.1
 Summary: Library of streaming algorithms for processing massive data.
 Author-email: "Dr. Hoa Vu and Daniel Barnas" <danielbarn90@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2023 Dr. Hoa Vu and Daniel Barnas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `sketchlib-0.0.0/pyproject.toml` & `sketchlib-0.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sketchlib"
-version = "0.0.0"
+version = "0.0.1"
 description = "Library of streaming algorithms for processing massive data."
 readme = "README.md"
 authors = [{ name = "Dr. Hoa Vu and Daniel Barnas", email = "danielbarn90@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,28 +24,25 @@
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/db-gb/DataStreamSketches"
+
 [tool.bumpver]
-current_version = "2023.1001-alpha"
-version_pattern = "YYYY.BUILD[-TAG]"
+current_version = "0.0.1"
+version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
 ]
-"setup.py" = [
-    "{version}",
-    "{pep440_version}",
-]
 "README.md" = [
     "{version}",
     "{pep440_version}",
 ]
```

### Comparing `sketchlib-0.0.0/sketchlib.egg-info/PKG-INFO` & `sketchlib-0.0.1/sketchlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchlib
-Version: 0.0.0
+Version: 0.0.1
 Summary: Library of streaming algorithms for processing massive data.
 Author-email: "Dr. Hoa Vu and Daniel Barnas" <danielbarn90@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2023 Dr. Hoa Vu and Daniel Barnas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `sketchlib-0.0.0/sketchlib.egg-info/SOURCES.txt` & `sketchlib-0.0.1/sketchlib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 streamsketchlib/__init__.py
 streamsketchlib/bloom_filter.py
 streamsketchlib/cm_hh_cash_register.py
 streamsketchlib/count_min.py
 streamsketchlib/f0_bjkst.py
 streamsketchlib/f0_estimate.py
 streamsketchlib/f2_estimate.py
-streamsketchlib/heavy_hitters.py
 streamsketchlib/heavy_hitters_cm.py
 streamsketchlib/minhash.py
 streamsketchlib/misra_gries.py
 streamsketchlib/rsv_sampling.py
 tests/test_bloom_filter.py
 tests/test_count_min.py
 tests/test_f0_estimate.py
```

### Comparing `sketchlib-0.0.0/streamsketchlib/bloom_filter.py` & `sketchlib-0.0.1/streamsketchlib/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/streamsketchlib/cm_hh_cash_register.py` & `sketchlib-0.0.1/streamsketchlib/cm_hh_cash_register.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from streamsketchlib.count_min import CountMin
 from heapq import heappush, heappop, heapify
-from heavy_hitters import AbstractHeavyHittersAlgorithm
 
 
-class HeavyHittersCMRegister(AbstractHeavyHittersAlgorithm):
+class HeavyHittersCMRegister:
     """ This class solves the heavy hitters problem using a count-min data
         structure. It works only for the cash register model of a stream where
         each token count must be greater than 0 (c > 0)."""
     def __init__(self, phi=0.01, epsilon=0.1, delta=0.01):
         self.phi = phi
         self.epsilon = epsilon
         self.delta = delta
```

### Comparing `sketchlib-0.0.0/streamsketchlib/count_min.py` & `sketchlib-0.0.1/streamsketchlib/count_min.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/streamsketchlib/f0_bjkst.py` & `sketchlib-0.0.1/streamsketchlib/f0_bjkst.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/streamsketchlib/f0_estimate.py` & `sketchlib-0.0.1/streamsketchlib/f0_estimate.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/streamsketchlib/f2_estimate.py` & `sketchlib-0.0.1/streamsketchlib/f2_estimate.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/streamsketchlib/heavy_hitters_cm.py` & `sketchlib-0.0.1/streamsketchlib/heavy_hitters_cm.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/streamsketchlib/minhash.py` & `sketchlib-0.0.1/streamsketchlib/minhash.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/streamsketchlib/misra_gries.py` & `sketchlib-0.0.1/streamsketchlib/misra_gries.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/streamsketchlib/rsv_sampling.py` & `sketchlib-0.0.1/streamsketchlib/rsv_sampling.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/tests/test_bloom_filter.py` & `sketchlib-0.0.1/tests/test_bloom_filter.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/tests/test_count_min.py` & `sketchlib-0.0.1/tests/test_count_min.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/tests/test_f0_estimate.py` & `sketchlib-0.0.1/tests/test_f0_estimate.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/tests/test_f2_estimate.py` & `sketchlib-0.0.1/tests/test_f2_estimate.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.0/tests/test_hh_count_min.py` & `sketchlib-0.0.1/tests/test_hh_count_min.py`

 * *Files identical despite different names*

