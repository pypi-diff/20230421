# Comparing `tmp/dimensionality_reductions_jmsv-0.1.0.tar.gz` & `tmp/dimensionality_reductions_jmsv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimensionality_reductions_jmsv-0.1.0.tar", max compression
+gzip compressed data, was "dimensionality_reductions_jmsv-0.2.0.tar", max compression
```

## Comparing `dimensionality_reductions_jmsv-0.1.0.tar` & `dimensionality_reductions_jmsv-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1085 2023-04-14 02:13:57.998461 dimensionality_reductions_jmsv-0.1.0/LICENSE
--rw-r--r--   0        0        0      959 2023-04-14 16:29:01.890515 dimensionality_reductions_jmsv-0.1.0/README.md
--rw-r--r--   0        0        0       51 2023-04-14 16:00:27.169349 dimensionality_reductions_jmsv-0.1.0/dimensionality_reductions_jmsv/__init__.py
--rw-r--r--   0        0        0     1334 2023-04-14 03:29:40.336579 dimensionality_reductions_jmsv-0.1.0/dimensionality_reductions_jmsv/decomposition/_PCA.py
--rw-r--r--   0        0        0      409 2023-04-14 08:11:38.699395 dimensionality_reductions_jmsv-0.1.0/dimensionality_reductions_jmsv/decomposition/_SVD.py
--rw-r--r--   0        0        0       98 2023-04-14 16:00:27.167263 dimensionality_reductions_jmsv-0.1.0/dimensionality_reductions_jmsv/decomposition/__init__.py
--rw-r--r--   0        0        0       40 2023-04-14 06:04:11.267984 dimensionality_reductions_jmsv-0.1.0/dimensionality_reductions_jmsv/manifold/_TSNE.py
--rw-r--r--   0        0        0       49 2023-04-14 16:00:27.165078 dimensionality_reductions_jmsv-0.1.0/dimensionality_reductions_jmsv/manifold/__init__.py
--rw-r--r--   0        0        0      743 2023-04-14 16:29:01.886669 dimensionality_reductions_jmsv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 dimensionality_reductions_jmsv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-14 02:13:57.998461 dimensionality_reductions_jmsv-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1826 2023-04-21 00:18:24.582930 dimensionality_reductions_jmsv-0.2.0/README.md
+-rw-r--r--   0        0        0       67 2023-04-15 16:31:23.848976 dimensionality_reductions_jmsv-0.2.0/dimensionality_reductions_jmsv/__init__.py
+-rw-r--r--   0        0        0     3028 2023-04-20 06:35:40.313468 dimensionality_reductions_jmsv-0.2.0/dimensionality_reductions_jmsv/cluster/_KMeans.py
+-rw-r--r--   0        0        0     6411 2023-04-20 21:53:56.871110 dimensionality_reductions_jmsv-0.2.0/dimensionality_reductions_jmsv/cluster/_KMedoids.py
+-rw-r--r--   0        0        0      104 2023-04-20 05:39:52.204110 dimensionality_reductions_jmsv-0.2.0/dimensionality_reductions_jmsv/cluster/__init__.py
+-rw-r--r--   0        0        0     1334 2023-04-14 03:29:40.336579 dimensionality_reductions_jmsv-0.2.0/dimensionality_reductions_jmsv/decomposition/_PCA.py
+-rw-r--r--   0        0        0      409 2023-04-14 08:11:38.699395 dimensionality_reductions_jmsv-0.2.0/dimensionality_reductions_jmsv/decomposition/_SVD.py
+-rw-r--r--   0        0        0       98 2023-04-14 16:00:27.167263 dimensionality_reductions_jmsv-0.2.0/dimensionality_reductions_jmsv/decomposition/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-14 06:04:11.267984 dimensionality_reductions_jmsv-0.2.0/dimensionality_reductions_jmsv/manifold/_TSNE.py
+-rw-r--r--   0        0        0       49 2023-04-14 16:00:27.165078 dimensionality_reductions_jmsv-0.2.0/dimensionality_reductions_jmsv/manifold/__init__.py
+-rw-r--r--   0        0        0      876 2023-04-21 00:21:44.047420 dimensionality_reductions_jmsv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 dimensionality_reductions_jmsv-0.2.0/PKG-INFO
```

### Comparing `dimensionality_reductions_jmsv-0.1.0/LICENSE` & `dimensionality_reductions_jmsv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dimensionality_reductions_jmsv-0.1.0/dimensionality_reductions_jmsv/decomposition/_PCA.py` & `dimensionality_reductions_jmsv-0.2.0/dimensionality_reductions_jmsv/decomposition/_PCA.py`

 * *Files identical despite different names*

### Comparing `dimensionality_reductions_jmsv-0.1.0/pyproject.toml` & `dimensionality_reductions_jmsv-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "dimensionality_reductions_jmsv"
-version = "0.1.0"
-description = "Package with the PCA, SVD and t-SNE methods for dimensionality reduction"
+version = "0.2.0"
+description = "Package with the PCA, SVD and t-SNE methods for dimensionality reduction. It also contains the clustering algorithms K-Means and K-Medoids."
 license = "MIT"
 authors = ["Mauricio Sierra"]
 maintainers = ["Send_Mail <mauricio@gmail.com>"]
 readme = "README.md"
 
 homepage = "https://pypi.org/project/dimensionality_reductions_jmsv/#history"
 repository = "https://github.com/mauriciosierrav/dimensionality-reduction-jmsv.git"
 
-keywords = ["SVD", "PCA", "t-SNE"]
+keywords = ["SVD", "PCA", "t-SNE", "KMeans", "KMedoids"]
 
 classifiers = [
-    'Programming Language :: Python', ]
+    'Programming Language :: Python :: 3.10',
+    'Development Status :: 4 - Beta']
 
 packages = [{include = "dimensionality_reductions_jmsv"}]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

