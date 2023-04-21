# Comparing `tmp/ReplayTables-andnp-2.3.0.tar.gz` & `tmp/ReplayTables-andnp-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReplayTables-andnp-2.3.0.tar", last modified: Tue Apr 11 22:55:10 2023, max compression
+gzip compressed data, was "ReplayTables-andnp-2.4.0.tar", last modified: Fri Apr 21 21:30:06 2023, max compression
```

## Comparing `ReplayTables-andnp-2.3.0.tar` & `ReplayTables-andnp-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/README.md
--rw-r--r--   0        0        0     5174 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/Distributions.py
--rw-r--r--   0        0        0     2140 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/LagBuffer.py
--rw-r--r--   0        0        0     2311 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/PER.py
--rw-r--r--   0        0        0     3622 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/ReplayBuffer.py
--rw-r--r--   0        0        0     8232 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/Table.py
--rw-r--r--   0        0        0        0 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/__init__.py
--rw-r--r--   0        0        0     3416 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/_utils/MemoryWriter.py
--rw-r--r--   0        0        0     1772 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/_utils/RandDict.py
--rw-r--r--   0        0        0     3816 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/_utils/SumTree.py
--rw-r--r--   0        0        0        0 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/_utils/__init__.py
--rw-r--r--   0        0        0     1220 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/_utils/jit.py
--rw-r--r--   0        0        0      888 2023-04-11 22:55:09.579496 ReplayTables-andnp-2.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3076 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/test_LagBuffer.py
--rw-r--r--   0        0        0     1944 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/test_PER.py
--rw-r--r--   0        0        0     2679 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/test_ReplayBuffer.py
--rw-r--r--   0        0        0     1537 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/test_Table.py
--rw-r--r--   0        0        0     5621 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/test_View.py
--rw-r--r--   0        0        0        0 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     2987 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/utils/test_SumTree.py
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 ReplayTables-andnp-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/README.md
+-rw-r--r--   0        0        0     5174 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/Distributions.py
+-rw-r--r--   0        0        0     2140 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/LagBuffer.py
+-rw-r--r--   0        0        0     2388 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/PER.py
+-rw-r--r--   0        0        0     3622 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/ReplayBuffer.py
+-rw-r--r--   0        0        0     8232 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/Table.py
+-rw-r--r--   0        0        0        0 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/__init__.py
+-rw-r--r--   0        0        0     3416 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/_utils/MemoryWriter.py
+-rw-r--r--   0        0        0     1772 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/_utils/RandDict.py
+-rw-r--r--   0        0        0     3816 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/_utils/SumTree.py
+-rw-r--r--   0        0        0        0 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/_utils/__init__.py
+-rw-r--r--   0        0        0     1220 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/_utils/jit.py
+-rw-r--r--   0        0        0      888 2023-04-21 21:30:05.398145 ReplayTables-andnp-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3076 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/test_LagBuffer.py
+-rw-r--r--   0        0        0     2370 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/test_PER.py
+-rw-r--r--   0        0        0     2679 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/test_ReplayBuffer.py
+-rw-r--r--   0        0        0     1537 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/test_Table.py
+-rw-r--r--   0        0        0     5621 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/test_View.py
+-rw-r--r--   0        0        0        0 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2987 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/utils/test_SumTree.py
+-rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 ReplayTables-andnp-2.4.0/PKG-INFO
```

### Comparing `ReplayTables-andnp-2.3.0/ReplayTables/Distributions.py` & `ReplayTables-andnp-2.4.0/ReplayTables/Distributions.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/ReplayTables/LagBuffer.py` & `ReplayTables-andnp-2.4.0/ReplayTables/LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/ReplayTables/PER.py` & `ReplayTables-andnp-2.4.0/ReplayTables/PER.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,17 @@
         self._max_priority = 1e-16
 
     def _sample_idxs(self, n: int) -> np.ndarray:
         idxs = self._idx_dist.sample(self._rng, n)
         return np.asarray(idxs)
 
     def _update_dist(self, idx: int, /, **kwargs: Any):
-        if self._c.new_priority_mode == 'max':
+        if 'priority' in kwargs:
+            priority = kwargs['priority']
+        elif self._c.new_priority_mode == 'max':
             priority = self._max_priority
         elif self._c.new_priority_mode == 'mean':
             total_priority = self._idx_dist.tree.dim_total(self._p_dist.dim)
             priority = total_priority / self.size()
             if priority == 0:
                 priority = 1e-16
         else:
```

### Comparing `ReplayTables-andnp-2.3.0/ReplayTables/ReplayBuffer.py` & `ReplayTables-andnp-2.4.0/ReplayTables/ReplayBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/ReplayTables/Table.py` & `ReplayTables-andnp-2.4.0/ReplayTables/Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/ReplayTables/_utils/MemoryWriter.py` & `ReplayTables-andnp-2.4.0/ReplayTables/_utils/MemoryWriter.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/ReplayTables/_utils/RandDict.py` & `ReplayTables-andnp-2.4.0/ReplayTables/_utils/RandDict.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/ReplayTables/_utils/SumTree.py` & `ReplayTables-andnp-2.4.0/ReplayTables/_utils/SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/ReplayTables/_utils/jit.py` & `ReplayTables-andnp-2.4.0/ReplayTables/_utils/jit.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/pyproject.toml` & `ReplayTables-andnp-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "2.3.0"
+version = "2.4.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -22,15 +22,15 @@
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "ReplayTables-andnp"
-version = "2.3.0"
+version = "2.4.0"
 description = "A simple replay buffer implementation in python for sampling n-step trajectories"
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numba>=0.56.4",
     "numpy>=1.23.5",
```

### Comparing `ReplayTables-andnp-2.3.0/tests/test_LagBuffer.py` & `ReplayTables-andnp-2.4.0/tests/test_LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/tests/test_PER.py` & `ReplayTables-andnp-2.4.0/tests/test_PER.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,31 @@
         self.assertEqual(buffer.size(), 5)
 
         samples, _, _ = buffer.sample(1000)
         unique = np.unique(samples.b)
         unique.sort()
         self.assertTrue(np.all(unique == np.array([2, 3, 4, 5, 6])))
 
+    def test_priority_on_add(self):
+        rng = np.random.RandomState(0)
+        buffer = PrioritizedReplay(5, Data, rng)
+
+        d = Data(a=0.1, b=1)
+        buffer.add(d, priority=1)
+        d = Data(a=0.2, b=2)
+        buffer.add(d, priority=2)
+
+        batch, _, _ = buffer.sample(128)
+
+        b = np.sum(batch.b == 2)
+        a = np.sum(batch.b == 1)
+
+        self.assertEqual(b, 85)
+        self.assertEqual(a, 43)
+
     def test_pickeable(self):
         rng = np.random.RandomState(0)
         buffer = PrioritizedReplay(5, Data, rng)
 
         for i in range(5):
             buffer.add(Data(i, 2 * i))
```

### Comparing `ReplayTables-andnp-2.3.0/tests/test_ReplayBuffer.py` & `ReplayTables-andnp-2.4.0/tests/test_ReplayBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/tests/test_Table.py` & `ReplayTables-andnp-2.4.0/tests/test_Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/tests/test_View.py` & `ReplayTables-andnp-2.4.0/tests/test_View.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.3.0/tests/utils/test_SumTree.py` & `ReplayTables-andnp-2.4.0/tests/utils/test_SumTree.py`

 * *Files identical despite different names*

