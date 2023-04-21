# Comparing `tmp/czech_workdays_holidays-0.0.6.tar.gz` & `tmp/czech_workdays_holidays-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czech_workdays_holidays-0.0.6.tar", last modified: Fri Apr 21 16:21:42 2023, max compression
+gzip compressed data, was "czech_workdays_holidays-0.0.7.tar", last modified: Fri Apr 21 19:23:34 2023, max compression
```

## Comparing `czech_workdays_holidays-0.0.6.tar` & `czech_workdays_holidays-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 16:21:42.292797 czech_workdays_holidays-0.0.6/
--rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech_workdays_holidays-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1645 2023-04-21 16:21:42.291796 czech_workdays_holidays-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2023-04-21 15:26:41.000000 czech_workdays_holidays-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 16:21:42.290293 czech_workdays_holidays-0.0.6/czech_workdays_holidays.egg-info/
--rw-rw-rw-   0        0        0     1645 2023-04-21 16:21:42.000000 czech_workdays_holidays-0.0.6/czech_workdays_holidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-21 16:21:42.000000 czech_workdays_holidays-0.0.6/czech_workdays_holidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 16:21:42.000000 czech_workdays_holidays-0.0.6/czech_workdays_holidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 16:21:42.000000 czech_workdays_holidays-0.0.6/czech_workdays_holidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10243 2023-04-21 15:43:21.000000 czech_workdays_holidays-0.0.6/czech_workdays_holidays.py
--rw-rw-rw-   0        0        0      667 2023-04-21 16:21:16.000000 czech_workdays_holidays-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 16:21:42.292797 czech_workdays_holidays-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 16:21:42.290795 czech_workdays_holidays-0.0.6/test/
--rw-rw-rw-   0        0        0        0 2023-04-21 12:09:27.000000 czech_workdays_holidays-0.0.6/test/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:23:34.368021 czech_workdays_holidays-0.0.7/
+-rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech_workdays_holidays-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1645 2023-04-21 19:23:34.368021 czech_workdays_holidays-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2023-04-21 15:26:41.000000 czech_workdays_holidays-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 19:23:34.366021 czech_workdays_holidays-0.0.7/czech_workdays_holidays.egg-info/
+-rw-rw-rw-   0        0        0     1645 2023-04-21 19:23:34.000000 czech_workdays_holidays-0.0.7/czech_workdays_holidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-21 19:23:34.000000 czech_workdays_holidays-0.0.7/czech_workdays_holidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 19:23:34.000000 czech_workdays_holidays-0.0.7/czech_workdays_holidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-21 19:23:34.000000 czech_workdays_holidays-0.0.7/czech_workdays_holidays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-21 19:23:34.000000 czech_workdays_holidays-0.0.7/czech_workdays_holidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10243 2023-04-21 15:43:21.000000 czech_workdays_holidays-0.0.7/czech_workdays_holidays.py
+-rw-rw-rw-   0        0        0      706 2023-04-21 19:23:28.000000 czech_workdays_holidays-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 19:23:34.368021 czech_workdays_holidays-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 19:23:34.367021 czech_workdays_holidays-0.0.7/test/
+-rw-rw-rw-   0        0        0        0 2023-04-21 12:09:27.000000 czech_workdays_holidays-0.0.7/test/tests.py
```

### Comparing `czech_workdays_holidays-0.0.6/LICENSE` & `czech_workdays_holidays-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.0.6/PKG-INFO` & `czech_workdays_holidays-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech_workdays_holidays
-Version: 0.0.6
+Version: 0.0.7
 Summary: Czech Workdays and Holidays including work-restricted holidays
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `czech_workdays_holidays-0.0.6/README.md` & `czech_workdays_holidays-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.0.6/czech_workdays_holidays.egg-info/PKG-INFO` & `czech_workdays_holidays-0.0.7/czech_workdays_holidays.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech-workdays-holidays
-Version: 0.0.6
+Version: 0.0.7
 Summary: Czech Workdays and Holidays including work-restricted holidays
 Author-email: David Gamba <gamba.d@seznam.cz>
 Project-URL: Homepage, https://github.com/david-gamba/Czech-Working-Days
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `czech_workdays_holidays-0.0.6/czech_workdays_holidays.py` & `czech_workdays_holidays-0.0.7/czech_workdays_holidays.py`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.0.6/pyproject.toml` & `czech_workdays_holidays-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "czech_workdays_holidays"
-version = "0.0.6"
+version = "0.0.7"
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
 
+dependencies = ["requirements.txt"]
+
 [project.urls]
 "Homepage" = "https://github.com/david-gamba/Czech-Working-Days"
 "Bug Tracker" = "https://github.com/david-gamba/Czech-Working-Days/issues"
```

