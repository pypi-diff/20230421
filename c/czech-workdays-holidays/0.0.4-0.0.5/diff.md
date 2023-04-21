# Comparing `tmp/czech_workdays_holidays-0.0.4.tar.gz` & `tmp/czech-workdays-holidays-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czech_workdays_holidays-0.0.4.tar", last modified: Fri Apr 21 15:31:01 2023, max compression
+gzip compressed data, was "czech-workdays-holidays-0.0.5.tar", last modified: Fri Apr 21 15:33:51 2023, max compression
```

## Comparing `czech_workdays_holidays-0.0.4.tar` & `czech-workdays-holidays-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 15:31:01.686612 czech_workdays_holidays-0.0.4/
--rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech_workdays_holidays-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1640 2023-04-21 15:31:01.686612 czech_workdays_holidays-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2023-04-21 15:26:41.000000 czech_workdays_holidays-0.0.4/README.md
--rw-rw-rw-   0        0        0      112 2023-04-21 14:22:38.000000 czech_workdays_holidays-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      721 2023-04-21 15:31:01.687612 czech_workdays_holidays-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 15:31:01.674609 czech_workdays_holidays-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 15:31:01.680610 czech_workdays_holidays-0.0.4/src/Czech_Workdays_Holidays/
--rw-rw-rw-   0        0        0        0 2023-04-21 15:23:15.000000 czech_workdays_holidays-0.0.4/src/Czech_Workdays_Holidays/__init__.py
--rw-rw-rw-   0        0        0    10242 2023-04-21 13:37:49.000000 czech_workdays_holidays-0.0.4/src/Czech_Workdays_Holidays/czech_workdays_holidays.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:31:01.684610 czech_workdays_holidays-0.0.4/src/czech_workdays_holidays.egg-info/
--rw-rw-rw-   0        0        0     1640 2023-04-21 15:31:01.000000 czech_workdays_holidays-0.0.4/src/czech_workdays_holidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-04-21 15:31:01.000000 czech_workdays_holidays-0.0.4/src/czech_workdays_holidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 15:31:01.000000 czech_workdays_holidays-0.0.4/src/czech_workdays_holidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 15:31:01.000000 czech_workdays_holidays-0.0.4/src/czech_workdays_holidays.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 15:31:01.685612 czech_workdays_holidays-0.0.4/test/
--rw-rw-rw-   0        0        0        0 2023-04-21 12:09:27.000000 czech_workdays_holidays-0.0.4/test/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:33:51.096295 czech-workdays-holidays-0.0.5/
+-rw-rw-rw-   0        0        0     1072 2023-04-21 15:08:04.000000 czech-workdays-holidays-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1640 2023-04-21 15:33:51.096295 czech-workdays-holidays-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2023-04-21 15:26:41.000000 czech-workdays-holidays-0.0.5/README.md
+-rw-rw-rw-   0        0        0      112 2023-04-21 14:22:38.000000 czech-workdays-holidays-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      721 2023-04-21 15:33:51.097296 czech-workdays-holidays-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 15:33:51.083293 czech-workdays-holidays-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 15:33:51.089295 czech-workdays-holidays-0.0.5/src/Czech_Workdays_Holidays/
+-rw-rw-rw-   0        0        0        0 2023-04-21 15:23:15.000000 czech-workdays-holidays-0.0.5/src/Czech_Workdays_Holidays/__init__.py
+-rw-rw-rw-   0        0        0    10242 2023-04-21 13:37:49.000000 czech-workdays-holidays-0.0.5/src/Czech_Workdays_Holidays/czech_workdays_holidays.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:33:51.094295 czech-workdays-holidays-0.0.5/src/czech_workdays_holidays.egg-info/
+-rw-rw-rw-   0        0        0     1640 2023-04-21 15:33:51.000000 czech-workdays-holidays-0.0.5/src/czech_workdays_holidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-04-21 15:33:51.000000 czech-workdays-holidays-0.0.5/src/czech_workdays_holidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 15:33:51.000000 czech-workdays-holidays-0.0.5/src/czech_workdays_holidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-21 15:33:51.000000 czech-workdays-holidays-0.0.5/src/czech_workdays_holidays.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 15:33:51.095294 czech-workdays-holidays-0.0.5/test/
+-rw-rw-rw-   0        0        0        0 2023-04-21 12:09:27.000000 czech-workdays-holidays-0.0.5/test/tests.py
```

### Comparing `czech_workdays_holidays-0.0.4/LICENSE` & `czech-workdays-holidays-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.0.4/PKG-INFO` & `czech-workdays-holidays-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: czech_workdays_holidays
-Version: 0.0.4
+Name: czech-workdays-holidays
+Version: 0.0.5
 Summary: Czech Workdays and Holidays including work-restricted holidays
 Home-page: https://github.com/david-gamba/Czech-Working-Days
 Author: David Gamba
 Author-email: gamba.d@seznam.cz
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `czech_workdays_holidays-0.0.4/README.md` & `czech-workdays-holidays-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.0.4/setup.cfg` & `czech-workdays-holidays-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2063 7a65 6368 5f77 6f72 6b64 6179   = czech_workday
-00000020: 735f 686f 6c69 6461 7973 0d0a 7665 7273  s_holidays..vers
-00000030: 696f 6e20 3d20 302e 302e 340d 0a61 7574  ion = 0.0.4..aut
+00000010: 203d 2063 7a65 6368 2d77 6f72 6b64 6179   = czech-workday
+00000020: 732d 686f 6c69 6461 7973 0d0a 7665 7273  s-holidays..vers
+00000030: 696f 6e20 3d20 302e 302e 350d 0a61 7574  ion = 0.0.5..aut
 00000040: 686f 7220 3d20 4461 7669 6420 4761 6d62  hor = David Gamb
 00000050: 610d 0a61 7574 686f 725f 656d 6169 6c20  a..author_email 
 00000060: 3d20 6761 6d62 612e 6440 7365 7a6e 616d  = gamba.d@seznam
 00000070: 2e63 7a0d 0a64 6573 6372 6970 7469 6f6e  .cz..description
 00000080: 203d 2043 7a65 6368 2057 6f72 6b64 6179   = Czech Workday
 00000090: 7320 616e 6420 486f 6c69 6461 7973 2069  s and Holidays i
 000000a0: 6e63 6c75 6469 6e67 2077 6f72 6b2d 7265  ncluding work-re
```

### Comparing `czech_workdays_holidays-0.0.4/src/Czech_Workdays_Holidays/czech_workdays_holidays.py` & `czech-workdays-holidays-0.0.5/src/Czech_Workdays_Holidays/czech_workdays_holidays.py`

 * *Files identical despite different names*

### Comparing `czech_workdays_holidays-0.0.4/src/czech_workdays_holidays.egg-info/PKG-INFO` & `czech-workdays-holidays-0.0.5/src/czech_workdays_holidays.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czech-workdays-holidays
-Version: 0.0.4
+Version: 0.0.5
 Summary: Czech Workdays and Holidays including work-restricted holidays
 Home-page: https://github.com/david-gamba/Czech-Working-Days
 Author: David Gamba
 Author-email: gamba.d@seznam.cz
 Project-URL: Bug Tracker, https://github.com/david-gamba/Czech-Working-Days/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

