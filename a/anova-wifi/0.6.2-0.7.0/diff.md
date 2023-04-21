# Comparing `tmp/anova_wifi-0.6.2.tar.gz` & `tmp/anova_wifi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anova_wifi-0.6.2.tar", max compression
+gzip compressed data, was "anova_wifi-0.7.0.tar", max compression
```

## Comparing `anova_wifi-0.6.2.tar` & `anova_wifi-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-04-04 22:26:23.837126 anova_wifi-0.6.2/LICENSE
--rw-r--r--   0        0        0     4360 2023-04-04 22:26:23.837126 anova_wifi-0.6.2/README.md
--rw-r--r--   0        0        0     2220 2023-04-04 22:26:24.653135 anova_wifi-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      483 2023-04-04 22:26:24.617135 anova_wifi-0.6.2/src/anova_wifi/__init__.py
--rw-r--r--   0        0        0      185 2023-04-04 22:26:23.837126 anova_wifi-0.6.2/src/anova_wifi/exceptions.py
--rw-r--r--   0        0        0     4000 2023-04-04 22:26:23.837126 anova_wifi-0.6.2/src/anova_wifi/parser.py
--rw-r--r--   0        0        0     8095 2023-04-04 22:26:23.837126 anova_wifi-0.6.2/src/anova_wifi/precission_cooker.py
--rw-r--r--   0        0        0        0 2023-04-04 22:26:23.837126 anova_wifi-0.6.2/src/anova_wifi/py.typed
--rw-r--r--   0        0        0     5428 1970-01-01 00:00:00.000000 anova_wifi-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-21 12:31:26.765831 anova_wifi-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4360 2023-04-21 12:31:26.765831 anova_wifi-0.7.0/README.md
+-rw-r--r--   0        0        0     2220 2023-04-21 12:31:27.673852 anova_wifi-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      483 2023-04-21 12:31:27.633851 anova_wifi-0.7.0/src/anova_wifi/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-21 12:31:26.769831 anova_wifi-0.7.0/src/anova_wifi/exceptions.py
+-rw-r--r--   0        0        0     4000 2023-04-21 12:31:26.769831 anova_wifi-0.7.0/src/anova_wifi/parser.py
+-rw-r--r--   0        0        0     8095 2023-04-21 12:31:26.769831 anova_wifi-0.7.0/src/anova_wifi/precission_cooker.py
+-rw-r--r--   0        0        0        0 2023-04-21 12:31:26.769831 anova_wifi-0.7.0/src/anova_wifi/py.typed
+-rw-r--r--   0        0        0     5428 1970-01-01 00:00:00.000000 anova_wifi-0.7.0/PKG-INFO
```

### Comparing `anova_wifi-0.6.2/LICENSE` & `anova_wifi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anova_wifi-0.6.2/README.md` & `anova_wifi-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `anova_wifi-0.6.2/pyproject.toml` & `anova_wifi-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anova-wifi"
-version = "0.6.2"
+version = "0.7.0"
 description = "A package to get read only data from Anova precision cookers with wifi"
 authors = ["Luke <conway220@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/conway220/anova-wifi"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `anova_wifi-0.6.2/src/anova_wifi/parser.py` & `anova_wifi-0.7.0/src/anova_wifi/parser.py`

 * *Files identical despite different names*

### Comparing `anova_wifi-0.6.2/src/anova_wifi/precission_cooker.py` & `anova_wifi-0.7.0/src/anova_wifi/precission_cooker.py`

 * *Files identical despite different names*

### Comparing `anova_wifi-0.6.2/PKG-INFO` & `anova_wifi-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anova-wifi
-Version: 0.6.2
+Version: 0.7.0
 Summary: A package to get read only data from Anova precision cookers with wifi
 Home-page: https://github.com/conway220/anova-wifi
 License: MIT
 Author: Luke
 Author-email: conway220@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anova-wifi Version: 0.6.2 Summary: A package to get
+Metadata-Version: 2.1 Name: anova-wifi Version: 0.7.0 Summary: A package to get
 read only data from Anova precision cookers with wifi Home-page: https://
 github.com/conway220/anova-wifi License: MIT Author: Luke Author-email:
 conway220@gmail.com Requires-Python: >=3.10,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

