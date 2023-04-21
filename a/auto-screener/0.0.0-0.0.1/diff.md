# Comparing `tmp/auto_screener-0.0.0.tar.gz` & `tmp/auto-screener-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_screener-0.0.0.tar", last modified: Fri Apr 21 17:38:31 2023, max compression
+gzip compressed data, was "auto-screener-0.0.1.tar", last modified: Fri Apr 21 17:54:54 2023, max compression
```

## Comparing `auto_screener-0.0.0.tar` & `auto-screener-0.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 17:38:31.003419 auto_screener-0.0.0/
--rw-rw-rw-   0        0        0      115 2023-04-21 17:38:30.000000 auto_screener-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-04-21 17:38:31.003419 auto_screener-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto_screener-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 17:38:30.985417 auto_screener-0.0.0/auto_screener/
--rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto_screener-0.0.0/auto_screener/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto_screener-0.0.0/auto_screener/base.py
--rw-rw-rw-   0        0        0     5939 2023-04-21 16:52:25.000000 auto_screener-0.0.0/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      526 2023-04-21 17:13:30.000000 auto_screener-0.0.0/auto_screener/document.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto_screener-0.0.0/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto_screener-0.0.0/auto_screener/interval.py
--rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto_screener-0.0.0/auto_screener/progress.py
--rw-rw-rw-   0        0        0    44904 2023-04-21 17:25:39.000000 auto_screener-0.0.0/auto_screener/screening.py
--rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto_screener-0.0.0/auto_screener/tickers.py
-drwxrwxrwx   0        0        0        0 2023-04-21 17:38:31.002451 auto_screener-0.0.0/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-04-21 17:38:30.000000 auto_screener-0.0.0/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-21 17:38:30.000000 auto_screener-0.0.0/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 17:38:30.000000 auto_screener-0.0.0/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-21 17:38:30.000000 auto_screener-0.0.0/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-21 17:38:30.000000 auto_screener-0.0.0/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto_screener-0.0.0/build.py
--rw-rw-rw-   0        0        0      645 2023-04-21 11:53:59.000000 auto_screener-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-04-21 17:11:58.000000 auto_screener-0.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 17:38:31.003419 auto_screener-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1655 2023-04-21 11:52:43.000000 auto_screener-0.0.0/setup.py
--rw-rw-rw-   0        0        0     1497 2023-04-21 17:37:38.000000 auto_screener-0.0.0/test.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:54:54.974085 auto-screener-0.0.1/
+-rw-rw-rw-   0        0        0      115 2023-04-21 17:54:54.000000 auto-screener-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-04-21 17:54:54.973084 auto-screener-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 17:54:54.957548 auto-screener-0.0.1/auto_screener/
+-rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto-screener-0.0.1/auto_screener/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.0.1/auto_screener/base.py
+-rw-rw-rw-   0        0        0     5939 2023-04-21 16:52:25.000000 auto-screener-0.0.1/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      526 2023-04-21 17:13:30.000000 auto-screener-0.0.1/auto_screener/document.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.0.1/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.0.1/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto-screener-0.0.1/auto_screener/progress.py
+-rw-rw-rw-   0        0        0    44904 2023-04-21 17:25:39.000000 auto-screener-0.0.1/auto_screener/screening.py
+-rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto-screener-0.0.1/auto_screener/tickers.py
+drwxrwxrwx   0        0        0        0 2023-04-21 17:54:54.973084 auto-screener-0.0.1/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-04-21 17:54:54.000000 auto-screener-0.0.1/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-21 17:54:54.000000 auto-screener-0.0.1/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 17:54:54.000000 auto-screener-0.0.1/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 17:54:54.000000 auto-screener-0.0.1/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-21 17:54:54.000000 auto-screener-0.0.1/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.0.1/build.py
+-rw-rw-rw-   0        0        0      645 2023-04-21 17:54:54.000000 auto-screener-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-04-21 17:54:19.000000 auto-screener-0.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 17:54:54.974085 auto-screener-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1655 2023-04-21 17:54:48.000000 auto-screener-0.0.1/setup.py
+-rw-rw-rw-   0        0        0     1497 2023-04-21 17:37:38.000000 auto-screener-0.0.1/test.py
```

### Comparing `auto_screener-0.0.0/PKG-INFO` & `auto-screener-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: auto_screener
-Version: 0.0.0
+Name: auto-screener
+Version: 0.0.1
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto_screener-0.0.0/README.md` & `auto-screener-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `auto_screener-0.0.0/auto_screener/base.py` & `auto-screener-0.0.1/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto_screener-0.0.0/auto_screener/dataset.py` & `auto-screener-0.0.1/auto_screener/dataset.py`

 * *Files identical despite different names*

### Comparing `auto_screener-0.0.0/auto_screener/document.py` & `auto-screener-0.0.1/auto_screener/document.py`

 * *Files identical despite different names*

### Comparing `auto_screener-0.0.0/auto_screener/interval.py` & `auto-screener-0.0.1/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto_screener-0.0.0/auto_screener/progress.py` & `auto-screener-0.0.1/auto_screener/progress.py`

 * *Files identical despite different names*

### Comparing `auto_screener-0.0.0/auto_screener/screening.py` & `auto-screener-0.0.1/auto_screener/screening.py`

 * *Files identical despite different names*

### Comparing `auto_screener-0.0.0/auto_screener/tickers.py` & `auto-screener-0.0.1/auto_screener/tickers.py`

 * *Files identical despite different names*

### Comparing `auto_screener-0.0.0/auto_screener.egg-info/PKG-INFO` & `auto-screener-0.0.1/auto_screener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.0
+Version: 0.0.1
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto_screener-0.0.0/build.py` & `auto-screener-0.0.1/build.py`

 * *Files identical despite different names*

### Comparing `auto_screener-0.0.0/pyproject.toml` & `auto-screener-0.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = 'auto_screener'
-version = '0.0.0'
+name = 'auto-screener'
+version = '0.0.1'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto_screener-0.0.0/setup.py` & `auto-screener-0.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         ],
         include=[
             "test.py",
             "auto_screener/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
-        name='auto_screener',
-        version='0.0.0',
+        name='auto-screener',
+        version='0.0.1',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `auto_screener-0.0.0/test.py` & `auto-screener-0.0.1/test.py`

 * *Files identical despite different names*

