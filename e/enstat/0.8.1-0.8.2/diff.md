# Comparing `tmp/enstat-0.8.1.tar.gz` & `tmp/enstat-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstat-0.8.1.tar", last modified: Fri Feb 24 10:11:50 2023, max compression
+gzip compressed data, was "enstat-0.8.2.tar", last modified: Thu Apr 20 13:39:49 2023, max compression
```

## Comparing `enstat-0.8.1.tar` & `enstat-0.8.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:11:50.230260 enstat-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:11:50.226260 enstat-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:11:50.230260 enstat-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-24 10:11:33.000000 enstat-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-24 10:11:33.000000 enstat-0.8.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-24 10:11:33.000000 enstat-0.8.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-02-24 10:11:33.000000 enstat-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-24 10:11:33.000000 enstat-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-24 10:11:33.000000 enstat-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-24 10:11:33.000000 enstat-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-24 10:11:50.230260 enstat-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-02-24 10:11:33.000000 enstat-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:11:50.230260 enstat-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-24 10:11:33.000000 enstat-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-24 10:11:33.000000 enstat-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-24 10:11:33.000000 enstat-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-24 10:11:33.000000 enstat-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-24 10:11:33.000000 enstat-0.8.1/docs/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:11:50.230260 enstat-0.8.1/enstat/
--rw-r--r--   0 runner    (1001) docker     (123)    22220 2023-02-24 10:11:33.000000 enstat-0.8.1/enstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-24 10:11:50.000000 enstat-0.8.1/enstat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-02-24 10:11:33.000000 enstat-0.8.1/enstat/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-02-24 10:11:33.000000 enstat-0.8.1/enstat/mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:11:50.230260 enstat-0.8.1/enstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-24 10:11:50.000000 enstat-0.8.1/enstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-24 10:11:50.000000 enstat-0.8.1/enstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 10:11:50.000000 enstat-0.8.1/enstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-24 10:11:50.000000 enstat-0.8.1/enstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-24 10:11:50.000000 enstat-0.8.1/enstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-24 10:11:33.000000 enstat-0.8.1/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 10:11:50.230260 enstat-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-24 10:11:33.000000 enstat-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:11:50.230260 enstat-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 10:11:33.000000 enstat-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-02-24 10:11:33.000000 enstat-0.8.1/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-02-24 10:11:33.000000 enstat-0.8.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:39:49.507664 enstat-0.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:39:49.503664 enstat-0.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:39:49.507664 enstat-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-20 13:39:32.000000 enstat-0.8.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-20 13:39:32.000000 enstat-0.8.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 13:39:32.000000 enstat-0.8.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-20 13:39:32.000000 enstat-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-20 13:39:32.000000 enstat-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-20 13:39:32.000000 enstat-0.8.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 13:39:32.000000 enstat-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-20 13:39:49.507664 enstat-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-20 13:39:32.000000 enstat-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:39:49.507664 enstat-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-20 13:39:32.000000 enstat-0.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 13:39:32.000000 enstat-0.8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-20 13:39:32.000000 enstat-0.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-20 13:39:32.000000 enstat-0.8.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-20 13:39:32.000000 enstat-0.8.2/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:39:49.507664 enstat-0.8.2/enstat/
+-rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-04-20 13:39:32.000000 enstat-0.8.2/enstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 13:39:49.000000 enstat-0.8.2/enstat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-20 13:39:32.000000 enstat-0.8.2/enstat/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-20 13:39:32.000000 enstat-0.8.2/enstat/mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:39:49.507664 enstat-0.8.2/enstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-20 13:39:49.000000 enstat-0.8.2/enstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-20 13:39:49.000000 enstat-0.8.2/enstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:39:49.000000 enstat-0.8.2/enstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 13:39:49.000000 enstat-0.8.2/enstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 13:39:49.000000 enstat-0.8.2/enstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 13:39:32.000000 enstat-0.8.2/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:39:49.507664 enstat-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-20 13:39:32.000000 enstat-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:39:49.507664 enstat-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:39:32.000000 enstat-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-20 13:39:32.000000 enstat-0.8.2/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-04-20 13:39:32.000000 enstat-0.8.2/tests/test_main.py
```

### Comparing `enstat-0.8.1/.github/workflows/ci.yml` & `enstat-0.8.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/.github/workflows/pre-commit.yml` & `enstat-0.8.2/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/.github/workflows/python-publish.yml` & `enstat-0.8.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/.gitignore` & `enstat-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/.pre-commit-config.yaml` & `enstat-0.8.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 repos:
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.3.0
   hooks:
   - id: black
     args: [--safe, --quiet, --line-length=100]
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-yaml
   - id: debug-statements
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.7.0
+  rev: v2.8.0
   hooks:
   - id: pretty-format-yaml
     args: [--preserve-quotes, --autofix, --indent, '2']
 - repo: https://github.com/humitos/mirrors-autoflake.git
   rev: v1.1
   hooks:
   - id: autoflake
```

### Comparing `enstat-0.8.1/LICENSE` & `enstat-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/PKG-INFO` & `enstat-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.8.1
+Version: 0.8.2
 Summary: Ensemble averages
 Home-page: https://github.com/tdegeus/enstat
 Author: Tom de Geus
 Author-email: tom@geus.me
 License: MIT
 Keywords: Statistics,Ensemble
 Description-Content-Type: text/markdown
```

### Comparing `enstat-0.8.1/README.md` & `enstat-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/docs/Makefile` & `enstat-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/docs/make.bat` & `enstat-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/docs/module.rst` & `enstat-0.8.2/docs/module.rst`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/enstat/__init__.py` & `enstat-0.8.2/enstat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,14 +509,15 @@
         bins: int = None,
         mode: str = "equal",
         min_count: int = None,
         min_width: float = None,
         integer: bool = False,
         bin_edges: ArrayLike = None,
         bound_error: str = "raise",
+        roundoff_error: float = 3.0 * np.finfo(np.float64).eps,
     ):
         r"""
         Construct a histogram from data.
 
         :param data: Data (flattened).
         :param bins: Number of bins.
         :param mode:
@@ -538,14 +539,16 @@
 
         :param bound_error: What to do if a sample falls out of the bin range:
 
             - ``"raise"``: raise an error
             - ``"ignore"``: ignore the data that are out of range
             - ``"norm"``: change the normalisation of the density
 
+        :param roundoff_error: Extend the first and last bin with this margin.
+
         :return: The :py:class:`Histogram` object.
         """
 
         if hasattr(bins, "__len__"):
             raise OSError("Only the number of bins can be specified")
 
         if bin_edges is None:
@@ -557,16 +560,16 @@
         if min_width is not None:
             bin_edges = detail.histogram_bin_edges_minwidth(bin_edges, min_width)
 
         if integer:
             bin_edges = detail.histogram_bin_edges_integer(bin_edges)
 
         bin_edges = np.array(bin_edges)
-        bin_edges[0] -= np.finfo(bin_edges.dtype).eps
-        bin_edges[-1] += np.finfo(bin_edges.dtype).eps
+        bin_edges[0] -= roundoff_error
+        bin_edges[-1] += roundoff_error
         return cls(bin_edges, right=True, bound_error=bound_error).add_sample(data)
 
     def strip(self, min_count: int = 0):
         """
         Strip the histogram of empty bins to the left and the right.
 
         :param min_count: The minimum count for a bin to be considered non-empty.
@@ -699,15 +702,15 @@
 
     def add_sample(self, data: ArrayLike):
         """
         Add a sample to the histogram.
         You can also use the ``+`` operator.
         """
 
-        bin = np.digitize(data, self.bin_edges, self.right) - 1
+        bin = np.digitize(data, self.bin_edges, right=self.right) - 1
 
         left = bin < 0
         right = bin >= self.count.size
         nleft = np.sum(left)
         nright = np.sum(right)
         self.count_left += nleft
         self.count_right += nright
```

### Comparing `enstat-0.8.1/enstat/detail.py` & `enstat-0.8.2/enstat/detail.py`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/enstat/mean.py` & `enstat-0.8.2/enstat/mean.py`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/enstat.egg-info/PKG-INFO` & `enstat-0.8.2/enstat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.8.1
+Version: 0.8.2
 Summary: Ensemble averages
 Home-page: https://github.com/tdegeus/enstat
 Author: Tom de Geus
 Author-email: tom@geus.me
 License: MIT
 Keywords: Statistics,Ensemble
 Description-Content-Type: text/markdown
```

### Comparing `enstat-0.8.1/enstat.egg-info/SOURCES.txt` & `enstat-0.8.2/enstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/setup.py` & `enstat-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/tests/test_histogram.py` & `enstat-0.8.2/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `enstat-0.8.1/tests/test_main.py` & `enstat-0.8.2/tests/test_main.py`

 * *Files identical despite different names*

