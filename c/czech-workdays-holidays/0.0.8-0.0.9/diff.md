# Comparing `tmp/czech_workdays_holidays-0.0.8.tar.gz` & `tmp/czech_workdays_holidays-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czech_workdays_holidays-0.0.8.tar", last modified: Fri Apr 21 19:30:31 2023, max compression
+gzip compressed data, was "czech_workdays_holidays-0.0.9.tar", last modified: Fri Apr 21 19:37:44 2023, max compression
```

## Comparing `czech_workdays_holidays-0.0.8.tar` & `czech_workdays_holidays-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 19:30:31.965131 czech_workdays_holidays-0.0.8/
--rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech_workdays_holidays-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1645 2023-04-21 19:30:31.965131 czech_workdays_holidays-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2023-04-21 15:26:41.000000 czech_workdays_holidays-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 19:30:31.962131 czech_workdays_holidays-0.0.8/czech_workdays_holidays.egg-info/
--rw-rw-rw-   0        0        0     1645 2023-04-21 19:30:31.000000 czech_workdays_holidays-0.0.8/czech_workdays_holidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-21 19:30:31.000000 czech_workdays_holidays-0.0.8/czech_workdays_holidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 19:30:31.000000 czech_workdays_holidays-0.0.8/czech_workdays_holidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 19:30:31.000000 czech_workdays_holidays-0.0.8/czech_workdays_holidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10243 2023-04-21 15:43:21.000000 czech_workdays_holidays-0.0.8/czech_workdays_holidays.py
--rw-rw-rw-   0        0        0      721 2023-04-21 19:30:26.000000 czech_workdays_holidays-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 19:30:31.965131 czech_workdays_holidays-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 19:30:31.964131 czech_workdays_holidays-0.0.8/test/
--rw-rw-rw-   0        0        0        0 2023-04-21 12:09:27.000000 czech_workdays_holidays-0.0.8/test/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:37:44.449131 czech_workdays_holidays-0.0.9/
+-rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech_workdays_holidays-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1645 2023-04-21 19:37:44.448130 czech_workdays_holidays-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2023-04-21 15:26:41.000000 czech_workdays_holidays-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 19:37:44.446130 czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/
+-rw-rw-rw-   0        0        0     1645 2023-04-21 19:37:44.000000 czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-21 19:37:44.000000 czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 19:37:44.000000 czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-21 19:37:44.000000 czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10243 2023-04-21 15:43:21.000000 czech_workdays_holidays-0.0.9/czech_workdays_holidays.py
+-rw-rw-rw-   0        0        0      788 2023-04-21 19:37:38.000000 czech_workdays_holidays-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 19:37:44.449131 czech_workdays_holidays-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 19:37:44.447130 czech_workdays_holidays-0.0.9/test/
+-rw-rw-rw-   0        0        0        0 2023-04-21 12:09:27.000000 czech_workdays_holidays-0.0.9/test/tests.py
```

### Comparing `czech_workdays_holidays-0.0.8/LICENSE` & `czech_workdays_holidays-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.0.8/PKG-INFO` & `czech_workdays_holidays-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech_workdays_holidays
-Version: 0.0.8
+Version: 0.0.9
 Summary: Czech Workdays and Holidays including work-restricted holidays
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `czech_workdays_holidays-0.0.8/README.md` & `czech_workdays_holidays-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.0.8/czech_workdays_holidays.egg-info/PKG-INFO` & `czech_workdays_holidays-0.0.9/czech_workdays_holidays.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech-workdays-holidays
-Version: 0.0.8
+Version: 0.0.9
 Summary: Czech Workdays and Holidays including work-restricted holidays
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `czech_workdays_holidays-0.0.8/czech_workdays_holidays.py` & `czech_workdays_holidays-0.0.9/czech_workdays_holidays.py`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.0.8/pyproject.toml` & `czech_workdays_holidays-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 
 [build-system]
-requires = ["setuptools>=61.0",
-            "python-dateutil",
-            "six"]
+requires = [
+    "setuptools >= 42.0.0",
+    # Add other build system dependencies here
+    "python-dateutil >= 2.8.2",
+    "six >= 1.16.0"
+]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "czech_workdays_holidays"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="David Gamba", email="gamba.d@seznam.cz" },
 ]
 description = "Czech Workdays and Holidays including work-restricted holidays"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+
+
 [project.urls]
 "Homepage" = "https://github.com/david-gamba/Czech-Working-Days"
 "Bug Tracker" = "https://github.com/david-gamba/Czech-Working-Days/issues"
```

