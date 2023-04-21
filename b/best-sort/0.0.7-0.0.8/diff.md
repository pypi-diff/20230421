# Comparing `tmp/best-sort-0.0.7.tar.gz` & `tmp/best-sort-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "best-sort-0.0.7.tar", last modified: Sun Apr 16 17:23:11 2023, max compression
+gzip compressed data, was "best-sort-0.0.8.tar", last modified: Fri Apr 21 01:09:21 2023, max compression
```

## Comparing `best-sort-0.0.7.tar` & `best-sort-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      130 2023-03-17 22:46:27.922581 best-sort-0.0.7/README.md
--rw-r--r--   0        0        0      825 2023-04-16 17:04:49.991064 best-sort-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      133 2023-04-16 17:03:44.081356 best-sort-0.0.7/src/best_sort/__init__.py
--rw-r--r--   0        0        0      160 2023-04-16 17:23:11.952404 best-sort-0.0.7/src/best_sort/_version.py
--rw-r--r--   0        0        0       62 2023-04-09 18:27:39.497791 best-sort-0.0.7/src/best_sort/sort_algos/__init__.py
--rw-r--r--   0        0        0     1060 2023-03-23 02:30:20.768607 best-sort-0.0.7/src/best_sort/sort_algos/bubble_sort.py
--rw-r--r--   0        0        0     1086 2023-03-31 02:22:50.498076 best-sort-0.0.7/src/best_sort/sort_algos/insertion_sort.py
--rw-r--r--   0        0        0     1017 2023-04-06 00:41:43.248019 best-sort-0.0.7/src/best_sort/sort_algos/selection_sort.py
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 best-sort-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      130 2023-03-17 22:46:27.922581 best-sort-0.0.8/README.md
+-rw-r--r--   0        0        0      825 2023-04-16 17:04:49.991064 best-sort-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-04-16 17:03:44.081356 best-sort-0.0.8/src/best_sort/__init__.py
+-rw-r--r--   0        0        0      160 2023-04-21 01:09:21.516627 best-sort-0.0.8/src/best_sort/_version.py
+-rw-r--r--   0        0        0       62 2023-04-09 18:27:39.497791 best-sort-0.0.8/src/best_sort/sort_algos/__init__.py
+-rw-r--r--   0        0        0     1060 2023-03-23 02:30:20.768607 best-sort-0.0.8/src/best_sort/sort_algos/bubble_sort.py
+-rw-r--r--   0        0        0     1086 2023-03-31 02:22:50.498076 best-sort-0.0.8/src/best_sort/sort_algos/insertion_sort.py
+-rw-r--r--   0        0        0     1017 2023-04-06 00:41:43.248019 best-sort-0.0.8/src/best_sort/sort_algos/selection_sort.py
+-rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 best-sort-0.0.8/PKG-INFO
```

### Comparing `best-sort-0.0.7/pyproject.toml` & `best-sort-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `best-sort-0.0.7/src/best_sort/sort_algos/bubble_sort.py` & `best-sort-0.0.8/src/best_sort/sort_algos/bubble_sort.py`

 * *Files identical despite different names*

### Comparing `best-sort-0.0.7/src/best_sort/sort_algos/insertion_sort.py` & `best-sort-0.0.8/src/best_sort/sort_algos/insertion_sort.py`

 * *Files identical despite different names*

### Comparing `best-sort-0.0.7/src/best_sort/sort_algos/selection_sort.py` & `best-sort-0.0.8/src/best_sort/sort_algos/selection_sort.py`

 * *Files identical despite different names*

### Comparing `best-sort-0.0.7/PKG-INFO` & `best-sort-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: best-sort
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package to find the best sorting algorithm for given data.
 Keywords: sorting algorithm,sorting,best algorithm
 Author-email: Joey Wheeler <joewheeler2048@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

