# Comparing `tmp/oops-all-itertools-2.0.1.tar.gz` & `tmp/oops-all-itertools-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oops-all-itertools-2.0.1.tar", last modified: Tue Mar 28 09:07:10 2023, max compression
+gzip compressed data, was "oops-all-itertools-2.0.2.tar", last modified: Fri Apr 21 08:05:59 2023, max compression
```

## Comparing `oops-all-itertools-2.0.1.tar` & `oops-all-itertools-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,5 @@
--rw-r--r--   0        0        0     1334 2023-03-08 10:31:56.885362 oops-all-itertools-2.0.1/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      328 2023-03-08 10:31:56.866362 oops-all-itertools-2.0.1/.gitignore
--rw-r--r--   0        0        0     1050 2023-03-08 07:44:07.211401 oops-all-itertools-2.0.1/LICENSE
--rw-r--r--   0        0        0     1426 2023-03-28 09:02:07.028644 oops-all-itertools-2.0.1/README.rst
--rw-r--r--   0        0        0      634 2023-03-09 07:38:21.341476 oops-all-itertools-2.0.1/docs/Makefile
--rw-r--r--   0        0        0     1226 2023-03-09 07:58:03.392440 oops-all-itertools-2.0.1/docs/conf.py
--rw-r--r--   0        0        0      470 2023-03-11 07:19:57.284960 oops-all-itertools-2.0.1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-03-09 07:38:21.342693 oops-all-itertools-2.0.1/docs/make.bat
--rw-r--r--   0        0        0        6 2023-03-09 07:39:02.258509 oops-all-itertools-2.0.1/docs/requirements.txt
--rw-r--r--   0        0        0      150 2023-03-28 09:03:21.725996 oops-all-itertools-2.0.1/oops_all_itertools/__init__.py
--rw-r--r--   0        0        0     1188 2023-03-08 11:12:16.841235 oops-all-itertools-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       38 2023-03-08 10:42:37.980268 oops-all-itertools-2.0.1/setup.py
--rw-r--r--   0        0        0        0 2023-03-08 10:31:56.875466 oops-all-itertools-2.0.1/tests/__init__.py
--rw-r--r--   0        0        0      232 2023-03-08 10:31:56.910053 oops-all-itertools-2.0.1/tests/test_oops_all.py
--rw-r--r--   0        0        0      109 2023-03-08 10:31:56.880329 oops-all-itertools-2.0.1/tox.ini
--rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 oops-all-itertools-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1050 2023-03-08 07:44:07.211401 oops-all-itertools-2.0.2/LICENSE
+-rw-r--r--   0        0        0     1426 2023-03-28 09:02:07.028644 oops-all-itertools-2.0.2/README.rst
+-rw-r--r--   0        0        0      150 2023-04-21 08:04:55.738345 oops-all-itertools-2.0.2/oops_all_itertools/__init__.py
+-rw-r--r--   0        0        0     1188 2023-03-08 11:12:16.841235 oops-all-itertools-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 oops-all-itertools-2.0.2/PKG-INFO
```

### Comparing `oops-all-itertools-2.0.1/LICENSE` & `oops-all-itertools-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oops-all-itertools-2.0.1/README.rst` & `oops-all-itertools-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `oops-all-itertools-2.0.1/pyproject.toml` & `oops-all-itertools-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oops-all-itertools-2.0.1/PKG-INFO` & `oops-all-itertools-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oops-all-itertools
-Version: 2.0.1
+Version: 2.0.2
 Summary: itertools and more-itertools all in one namespace
 Keywords: itertools,iterator,iteration,filter,peek,peekable,chunk,chunked
 Author: Lonnen
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

